---
title: Iskanje vsebine ni rezultat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680663"
---
# <a name="no-results-from-content-searchexports"></a>Ni rezultatov iskanja/izvoza vsebine

Težave z iskanjem/izvozom vsebine ne vračajo nobenih podatkov je morda zaradi določenega filtra varnosti skladnosti, ki ga je nastavil določen skrbnik in ga ni mogoče sporočiti vsem skrbnikom.

To težavo odpravite tako, da preverite, ali obstajajo filtri varnosti skladnosti, ki jih lahko povzroči to:
1. Vzpostavljanje povezave z lupino PowerShell za varnost in skladnost s predpisi
2. Zaženite ta ukazov:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizacija $org