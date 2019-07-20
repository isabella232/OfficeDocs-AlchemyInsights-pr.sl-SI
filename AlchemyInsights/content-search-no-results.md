---
title: Vsebine ne rezultati iskanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800602"
---
# <a name="no-results-from-content-searchexports"></a>Ni rezultatov iz vsebine iskanje/izvoz

Vprašanja z vsebino iskanje/izvoz ne vračajo podatkov je lahko posledica nekaterih skladnosti varnostnega filtra, da je bila namestitev posebnih Admin in ne komunicira vse administratorji.

Če želite to odpraviti, preverite, če obstajajo kakršne koli skladnosti varnostnih filtrov, ki lahko povzroča to:
1. Povezati varnost in skladnost Center Powershell
2. Zaženite naslednje commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizacija $org