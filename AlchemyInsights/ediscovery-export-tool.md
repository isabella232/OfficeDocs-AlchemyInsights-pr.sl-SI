---
title: Orodje za izvoz e-odkrivanja
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814604"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="505fe-102">Ali ne morete namestiti ali zagnati orodja za izvoz e-odkrivanja?</span><span class="sxs-lookup"><span data-stu-id="505fe-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="505fe-103">Če ne morete namestiti ali zagnati orodja za izvoz e-odkrivanja, da bi prenesli rezultate iskanja, preverite te elemente:</span><span class="sxs-lookup"><span data-stu-id="505fe-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="505fe-104">Računalnik, ki ga uporabljate, izpolnjuje te zahteve:</span><span class="sxs-lookup"><span data-stu-id="505fe-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="505fe-105">32- ali 64-bitne različice sistema Windows 7 in novejše različice</span><span class="sxs-lookup"><span data-stu-id="505fe-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="505fe-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="505fe-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="505fe-107">Podprt brskalnik:</span><span class="sxs-lookup"><span data-stu-id="505fe-107">A supported browser:</span></span>

  - <span data-ttu-id="505fe-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="505fe-108">Microsoft Edge</span></span>

    <span data-ttu-id="505fe-109">Ali</span><span class="sxs-lookup"><span data-stu-id="505fe-109">Or</span></span>

  - <span data-ttu-id="505fe-110">Internet Explorer 10 in novejše različice</span><span class="sxs-lookup"><span data-stu-id="505fe-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="505fe-111">Drugi brskalniki, kot sta Google Chrome in Mozilla Firefox, niso podprti.</span><span class="sxs-lookup"><span data-stu-id="505fe-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="505fe-112">Vaša organizacija se lahko poveže s končno točko v storitvi Azure, ki je **\* .blob.core.windows.net** (nadomestni znak predstavlja enolični identifikator za posel izvoza).</span><span class="sxs-lookup"><span data-stu-id="505fe-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="505fe-113">Dodeljena vam je vloga za izvoz v Središču za varnost in skladnost s predpisi storitve Microsoft 365. &amp;</span><span class="sxs-lookup"><span data-stu-id="505fe-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="505fe-114">Privzeto je ta vloga dodeljena le skupini vlog upravitelja e-odkrivanja.</span><span class="sxs-lookup"><span data-stu-id="505fe-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="505fe-115">Glejte [Dodeljevanje dovoljenj za e-odkrivanje.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="505fe-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="505fe-116">Če želite več informacij, glejte [Izvoz rezultatov iskanja po vsebini.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="505fe-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="505fe-117">Če izvažate več kot 100.000 nabiralnikov, morate za prenos rezultatov izvoza uporabiti to storitev Powershell: Izvoz rezultatov iz več kot [100 K nabiralnikov.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="505fe-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>