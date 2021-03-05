---
title: Težava z filtrom» atribut «in» določanje obsega «
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482922"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Težava z filtrom» atribut «in» določanje obsega «

**Težave s spornimi vrednostmi UPN**

Delovni dan za omogočanje uporabe delovnega dne na spletnem mestu AD uporabnik omogoča omogočanje uporabe sporočila o napaki **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Operacija ni uspela, ker vrednost UPN za dodatek/spreminjanje ni enolična za celotno vrsto gozda. Podrobnosti o napaki: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

Vrednost **userPrincipalName** , ki jo priključek delovnega dne poskuša nastaviti, ko ustvarja uporabniški račun oglasa že obstaja v ciljni domeni oglasa. To pomeni, da uporabnik že obstaja in preverjanje ujemanja ID-ja ni uspelo za uporabnika ali (2) pravilo generiranja UPN je ustvarilo sporno vrednost.

Tukaj so navodila za predlagano rešitev:

Če uporabnik že obstaja in preverjanje ujemanja ID-ja ni uspelo povezati računa za delovni dan z računom imenika Active Directory, nato preverite, ali je atribut» ujemanje ID-ja «(običajno **IDzaposlenega**) v obeh delovnih dneh in ad natančno ujemanje. Če se ne ujemajo, je to podatkovna težava, ki jo je treba popraviti. Če je na primer IDZaposlenega v delovnem programu 001052 in je v OGLASu 1052, potem mehanizem za omogočanje uporabe ne bo mogel povezati dveh računov in bo poskušal ustvariti uporabnika, ki že obstaja. Rešitev v tem primeru je, da spremenite vrednost **IDzaposlenega** v programu ad, da vključite vodilne ničle, da bo 001052.
Če izraz, ki ustvarja UPN, ne ustvari enolične vrednosti, uporabite funkcijo de-podvajanja **SelectUniqueValue** , da vsakič ustvarite enolično vrednost.

**Delovni dan za omogočanje uporabe uporabnika ne Nastavi vrednosti atributa upravitelja za uporabniški račun OGLASa**

Posel za omogočanje uporabe uporabnika delovnega dne v OGLASu ne določa vrednosti atributa **upravitelja** za UPORABNIŠKE račune oglasa. Ko je to vedenje prikazano, sta na voljo dva možna scenarija:

1. Upravitelja v delavniku ni mogoče razrešiti z ustreznim uporabniškim računom OGLASa, ker upravitelj ni v obsegu.
2. V scenariju z **več domenami oglasa** upravitelj v delovnem programu ni prisoten v isti domeni kot uporabnik.

Če želite odpraviti težavo, poskusite s temi koraki:

1. Če ste določili filtre za določanje obsega, najprej preverite, ali je upravitelj v obsegu in ali ustreza stavku za določanje obsega. Če upravitelj ne izpolnjuje filtra za določanje obsega, spremenite filter tako, da je upravitelj tudi v obsegu uporabe postopka uporabe.
2. Če imate več domen oglasov, ima povezovalnik znano omejitev nezmožnosti za razreševanje sklicev upravitelja navzkrižne domene.

Če želite več informacij o konfiguriranju delovnega dne za avtomatizirano omogočanje uporabe, glejte [Vadnica: konfiguracija delovnega dne za samodejno omogočanje uporabe uporabnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













