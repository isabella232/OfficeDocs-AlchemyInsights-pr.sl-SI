---
title: Med iskanjem/izvozom vsebine ni vrnjenih rezultatov
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101282"
---
# <a name="no-results-returned-during-content-searchexport"></a>Med iskanjem/izvozom vsebine ni vrnjenih rezultatov

Če prihaja do težav s tem scenarijem e-odkrivanja:

- Iskanje vsebine/izvoz ne vrne nobenih podatkov ali nepričakovanih podatkov
- Iskanje z e-odkrivanjem ali izvozom ne uspe

Do tega lahko pride zaradi določenih varnostnih filtrov za skladnost s predpisi, ki jih je nastavite določen skrbnik in niso bili posredovani vsem skrbnikom.

Če želite odpraviti to težavo, preverite, ali obstajajo morda kateri koli varnostni filtri za skladnost s predpisi, ki povzročajo te težave:

1. Povezovalnik v Središče za varnost in skladnost s predpisi Powershell
2. Zaženite te ukazne vrstice:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Če želite več informacij o varnostnih filtrih za skladnost s predpisi, [glejte Filtriranje dovoljenj za iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
