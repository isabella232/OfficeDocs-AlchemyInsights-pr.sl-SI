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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727239"
---
# <a name="no-results-returned-during-content-searchexport"></a>Med iskanjem in izvozom vsebine ni vrnjenih rezultatov

Če imate težave s temi E-odkrivanje scenariji:

- Iskanje vsebine/izvoz vrne brez podatkov ali nepričakovanih podatkov
- E-odkrivanje iskanje ali izvoz ne uspe

To je morda zaradi nekaterih varnostnih filtrov skladnosti, ki jih je nastavil določen skrbnik in niso bili posredovani vsem skrbnikom.

To težavo odpravite tako, da preverite, ali obstajajo filtri varnosti skladnosti, ki morda povzročajo te težave:

1. Vzpostavljanje povezave z lupino PowerShell za varnost in skladnost s predpisi
2. Zaženite ta ukazov:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Če želite več informacij o varnostnih filtrih skladnosti, glejte [filtriranje dovoljenj za iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
