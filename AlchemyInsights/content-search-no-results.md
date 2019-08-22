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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516795"
---
# <a name="no-results-from-content-searchexports"></a>Ni rezultatov iz vsebine iskanje/izvoz

Vprašanja z vsebino iskanje/izvoz ne vračajo podatkov je lahko posledica nekaterih skladnosti varnostnega filtra, da je bila namestitev posebnih Admin in ne komunicira vse administratorji.

Če želite to odpraviti, preverite, če obstajajo kakršne koli skladnosti varnostnih filtrov, ki lahko povzroča to:
1. Povezati varnost in skladnost Center Powershell
2. Zaženite naslednje commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-organizacija $org