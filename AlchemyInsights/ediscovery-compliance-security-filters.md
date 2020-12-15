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
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="ec251-102">Med iskanjem in izvozom vsebine ni vrnjenih rezultatov</span><span class="sxs-lookup"><span data-stu-id="ec251-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="ec251-103">Če imate težave s temi E-odkrivanje scenariji:</span><span class="sxs-lookup"><span data-stu-id="ec251-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="ec251-104">Iskanje vsebine/izvoz vrne brez podatkov ali nepričakovanih podatkov</span><span class="sxs-lookup"><span data-stu-id="ec251-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="ec251-105">E-odkrivanje iskanje ali izvoz ne uspe</span><span class="sxs-lookup"><span data-stu-id="ec251-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="ec251-106">Do tega lahko pride zaradi nekaterih filtrov varnosti skladnosti, ki jih je nastavil določen skrbnik in niso bili posredovani vsem skrbnikom.</span><span class="sxs-lookup"><span data-stu-id="ec251-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="ec251-107">To težavo odpravite tako, da preverite, ali obstajajo filtri varnosti skladnosti, ki morda povzročajo te težave:</span><span class="sxs-lookup"><span data-stu-id="ec251-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="ec251-108">Vzpostavljanje povezave z lupino PowerShell za varnost in skladnost s predpisi</span><span class="sxs-lookup"><span data-stu-id="ec251-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="ec251-109">Zaženite ta ukazov:</span><span class="sxs-lookup"><span data-stu-id="ec251-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="ec251-110">Če želite več informacij o varnostnih filtrih skladnosti, glejte [filtriranje dovoljenj za iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="ec251-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
