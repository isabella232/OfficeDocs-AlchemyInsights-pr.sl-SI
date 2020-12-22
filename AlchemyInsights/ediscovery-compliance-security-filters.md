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
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="ab4f7-102">Med iskanjem in izvozom vsebine ni vrnjenih rezultatov</span><span class="sxs-lookup"><span data-stu-id="ab4f7-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="ab4f7-103">Če imate težave s temi E-odkrivanje scenariji:</span><span class="sxs-lookup"><span data-stu-id="ab4f7-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="ab4f7-104">Iskanje vsebine/izvoz vrne brez podatkov ali nepričakovanih podatkov</span><span class="sxs-lookup"><span data-stu-id="ab4f7-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="ab4f7-105">E-odkrivanje iskanje ali izvoz ne uspe</span><span class="sxs-lookup"><span data-stu-id="ab4f7-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="ab4f7-106">To je morda zaradi nekaterih varnostnih filtrov skladnosti, ki jih je nastavil določen skrbnik in niso bili posredovani vsem skrbnikom.</span><span class="sxs-lookup"><span data-stu-id="ab4f7-106">This may be due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="ab4f7-107">To težavo odpravite tako, da preverite, ali obstajajo filtri varnosti skladnosti, ki morda povzročajo te težave:</span><span class="sxs-lookup"><span data-stu-id="ab4f7-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="ab4f7-108">Vzpostavljanje povezave z lupino PowerShell za varnost in skladnost s predpisi</span><span class="sxs-lookup"><span data-stu-id="ab4f7-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="ab4f7-109">Zaženite ta ukazov:</span><span class="sxs-lookup"><span data-stu-id="ab4f7-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="ab4f7-110">Če želite več informacij o varnostnih filtrih skladnosti, glejte [filtriranje dovoljenj za iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="ab4f7-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
