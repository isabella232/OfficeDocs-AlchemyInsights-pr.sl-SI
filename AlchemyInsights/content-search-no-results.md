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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058018"
---
# <a name="no-results-from-content-searchexports"></a>Ni rezultatov iskanja/izvoza vsebine

Težave z iskanjem vsebine/izvozi, ki ne vračajo nobenih podatkov, so lahko posledica določenega varnostnega filtra za skladnost s predpisi, ki ga je nastavljen določen skrbnik in ki je ne sporoča vsem skrbnikom.

Če želite odpraviti to težavo, preverite, ali obstajajo morda kateri koli varnostni filtri za skladnost s predpisi, ki povzročajo to:
1. Povezovalnik v Središče za varnost in skladnost s predpisi Powershell
2. Zaženite te ukazne vrstice:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter – organizacija $org