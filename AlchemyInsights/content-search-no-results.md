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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="f5468-102">Ni rezultatov iskanja/izvoza vsebine</span><span class="sxs-lookup"><span data-stu-id="f5468-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="f5468-103">Težave z iskanjem vsebine/izvozi, ki ne vračajo nobenih podatkov, so lahko posledica določenega varnostnega filtra za skladnost s predpisi, ki ga je nastavljen določen skrbnik in ki je ne sporoča vsem skrbnikom.</span><span class="sxs-lookup"><span data-stu-id="f5468-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="f5468-104">Če želite odpraviti to težavo, preverite, ali obstajajo morda kateri koli varnostni filtri za skladnost s predpisi, ki povzročajo to:</span><span class="sxs-lookup"><span data-stu-id="f5468-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="f5468-105">Povezovanje z lupino Powershell v Središču za varnost in skladnost s predpisi</span><span class="sxs-lookup"><span data-stu-id="f5468-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="f5468-106">Zaženite te ukazne vrstice:</span><span class="sxs-lookup"><span data-stu-id="f5468-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="f5468-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="f5468-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="f5468-108">Get-ComplianceSecurityFilter – organizacija $org</span><span class="sxs-lookup"><span data-stu-id="f5468-108">Get-ComplianceSecurityFilter -Organization $org</span></span>