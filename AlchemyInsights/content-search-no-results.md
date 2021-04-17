---
title: Content Search No Results
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816864"
---
# <a name="no-results-from-content-searchexports"></a>Ni rezultatov iskanja/izvoza vsebine

Težave z iskanjem vsebine/izvozi, ki ne vračajo nobenih podatkov, so lahko posledica določenega varnostnega filtra za skladnost s predpisi, ki ga je nastavljen določen skrbnik in ki je ne sporoča vsem skrbnikom.

Če želite odpraviti to težavo, preverite, ali obstajajo morda kateri koli varnostni filtri za skladnost s predpisi, ki povzročajo to:
1. Povezovanje z lupino Powershell v Središču za varnost in skladnost s predpisi
2. Zaženite te ukazne vrstice:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter – organizacija $org