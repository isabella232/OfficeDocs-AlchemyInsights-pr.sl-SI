---
title: Delovni dan do omogočanja uporabe uporabnika v karanteni
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482904"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Delovni dan do omogočanja uporabe uporabnika v karanteni

**Delovni dan za omogočanje uporabe uporabnika v sistemu AD gre v stanje karantene in uporabniki niso ustvarjeni v programu AD**

Posel za omogočanje uporabe uporabnika v programu AD je šel v stanje karantene in dnevniki nadzora kažejo dogodke izvozne neuspelosti z napako sporočila o napaki **: OperationsError-SvcErr: Prišlo je do napake v operaciji. Za imeniško storitev ni bil konfiguriran noben nadrejeni sklic. Imeniška storitev torej ne more izdajati napotitev predmetov zunaj tega gozda**. Ta napaka se običajno prikaže, če vsebnik imenika Active Directory OU ni nastavljen pravilno ali če so na voljo težave z izrazom preslikave izraza, ki se uporablja za **parentDistinguishedName**.

Preverite privzeti parameter OU za **nove uporabnike** za tipkarske napake. Zagotovite, da navedeni OU že obstaja v vašem OGLASu. Če v preslikavi atributov uporabljate **parentDistinguishedName** , zagotovite, da je vedno ovrednotena z znanim vsebnikom v domeni oglasa. Če želite videti ustvarjeno vrednost, v dnevnikih nadzora preverite dogodek izvoza.

Če želite več informacij o konfiguriranju delovnega dne za avtomatizirano omogočanje uporabe, glejte [Vadnica: konfiguracija delovnega dne za samodejno omogočanje uporabe uporabnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

