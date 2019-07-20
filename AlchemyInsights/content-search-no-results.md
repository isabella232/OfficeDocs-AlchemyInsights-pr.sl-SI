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
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="5a463-102">Ni rezultatov iz vsebine iskanje/izvoz</span><span class="sxs-lookup"><span data-stu-id="5a463-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="5a463-103">Vprašanja z vsebino iskanje/izvoz ne vračajo podatkov je lahko posledica nekaterih skladnosti varnostnega filtra, da je bila namestitev posebnih Admin in ne komunicira vse administratorji.</span><span class="sxs-lookup"><span data-stu-id="5a463-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="5a463-104">Če želite to odpraviti, preverite, če obstajajo kakršne koli skladnosti varnostnih filtrov, ki lahko povzroča to:</span><span class="sxs-lookup"><span data-stu-id="5a463-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="5a463-105">Povezati varnost in skladnost Center Powershell</span><span class="sxs-lookup"><span data-stu-id="5a463-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="5a463-106">Zaženite naslednje commandlets:</span><span class="sxs-lookup"><span data-stu-id="5a463-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="5a463-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="5a463-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="5a463-108">Get-ComplianceSecurityFilter-organizacija $org</span><span class="sxs-lookup"><span data-stu-id="5a463-108">Get-ComplianceSecurityFilter -Organization $org</span></span>