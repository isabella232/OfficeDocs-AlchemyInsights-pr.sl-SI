---
title: orodje za izvoz E-odkrivanje
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277944"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="c6d22-102">Ne morete namestiti ali zagnati orodja za izvoz E-odkrivanje?</span><span class="sxs-lookup"><span data-stu-id="c6d22-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="c6d22-103">Če ne morete namestiti ali zagnati orodja za izvoz E-odkrivanje za prenos rezultatov iskanja, si oglejte te stvari:</span><span class="sxs-lookup"><span data-stu-id="c6d22-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="c6d22-104">Računalnik, ki ga uporabljate, izpolnjuje te pogoje:</span><span class="sxs-lookup"><span data-stu-id="c6d22-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="c6d22-105">32-ali 64-bitne različice sistema Windows 7 in novejše različice</span><span class="sxs-lookup"><span data-stu-id="c6d22-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="c6d22-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="c6d22-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="c6d22-107">Podprt brskalnik:</span><span class="sxs-lookup"><span data-stu-id="c6d22-107">A supported browser:</span></span>

  - <span data-ttu-id="c6d22-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c6d22-108">Microsoft Edge</span></span>

    <span data-ttu-id="c6d22-109">Ali</span><span class="sxs-lookup"><span data-stu-id="c6d22-109">Or</span></span>

  - <span data-ttu-id="c6d22-110">Internet Explorer 10 in novejše različice</span><span class="sxs-lookup"><span data-stu-id="c6d22-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="c6d22-111">Drugi brskalniki, kot sta Google Chrome in Mozilla Firefox, niso podprti.</span><span class="sxs-lookup"><span data-stu-id="c6d22-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="c6d22-112">Vaša organizacija se lahko poveže s končno točko v storitvi Azure, ki je \*\* \* . blob.Core.Windows.net\*\* (nadomestni znak predstavlja Enolični identifikator za izvozno opravilo).</span><span class="sxs-lookup"><span data-stu-id="c6d22-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="c6d22-113">Izvozna vloga je dodeljena v središču za skladnost z varnostnim preverjanjem za Microsoft 365 &amp; .</span><span class="sxs-lookup"><span data-stu-id="c6d22-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="c6d22-114">Ta vloga je privzeto dodeljena le skupini vlog E-odkrivanje Manager.</span><span class="sxs-lookup"><span data-stu-id="c6d22-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="c6d22-115">Glejte [dodeljevanje dovoljenj za e-odkrivanje](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="c6d22-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="c6d22-116">Če želite več informacij, glejte [izvoz rezultatov iskanja vsebine](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="c6d22-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="c6d22-117">Če izvažate več kot 100K nabiralnike, boste morali uporabiti ta PowerShell za prenos rezultatov izvoza:  [izvažanje rezultatov iz več kot 100k nabiralnikov](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="c6d22-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>