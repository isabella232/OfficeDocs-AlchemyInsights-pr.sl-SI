---
title: Med iskanjem in izvozom vsebine ni vrnjenih rezultatov
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
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680328"
---
# <a name="no-results-returned-during-content-searchexport"></a>Med iskanjem in izvozom vsebine ni vrnjenih rezultatov

Če imate težave s temi E-odkrivanje scenariji:

- Iskanje vsebine/izvoz vrne brez podatkov ali nepričakovanih podatkov
- E-odkrivanje iskanje ali izvoz ne uspe

Do tega lahko pride zaradi nekaterih filtrov varnosti skladnosti, ki jih je nastavil določen skrbnik in niso bili posredovani vsem skrbnikom.

To težavo odpravite tako, da preverite, ali obstajajo filtri varnosti skladnosti, ki morda povzročajo te težave:

1. Vzpostavljanje povezave z lupino PowerShell za varnost in skladnost s predpisi
2. Zaženite ta ukazov:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Če želite več informacij o varnostnih filtrih skladnosti, glejte [filtriranje dovoljenj za iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
