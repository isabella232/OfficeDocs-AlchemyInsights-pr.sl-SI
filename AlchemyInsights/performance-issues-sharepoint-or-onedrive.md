---
title: Težave z učinkovitostjo delovanja – SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771917"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4bbde-102">SharePoint ali OneDrive počasno, nedostopno ali ni na voljo za več uporabnikov</span><span class="sxs-lookup"><span data-stu-id="4bbde-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="4bbde-103">SharePoint ali OneDrive je lahko počasno, nedostopno ali pa ni na voljo ali pa lahko prikaže storitev nedostopnih ali 503, iz več razlogov:</span><span class="sxs-lookup"><span data-stu-id="4bbde-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="4bbde-104">Če je SharePointovo ali OneDrive mesto počasno ali Zakasnjeno za več uporabnikov, je morda prišlo do začasne težave s storitvijo, kjer uporabniki občasno opazijo ponavljajoče se zamude ali napake pri krmarjenju, ko dostopajo do SharePointovih mest ali vsebine OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4bbde-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="4bbde-105">Preverite, ali je [Nadzorna plošča za zdravstveno stanje na voljo](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , če želite preveriti, ali je vaša organizacija vplivala nanje.</span><span class="sxs-lookup"><span data-stu-id="4bbde-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="4bbde-106">Uporabniki lahko prejmejo *strežnik 503,* ko poskušate krmariti do SharePointovih mest ali OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4bbde-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="4bbde-107">Do te napake lahko pride zaradi omejevanja v SharePointovi storitvi.</span><span class="sxs-lookup"><span data-stu-id="4bbde-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="4bbde-108">Storitev SharePoint Online z omejevanjem zmogljivosti vzdržuje optimalno učinkovitost in zanesljivost storitve SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4bbde-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="4bbde-109">Omejevanje zmogljivosti omeji število uporabniških dejanj ali sočasnih klicev (s skriptom ali kodo) in tako prepreči prekomerno uporabo sredstev.</span><span class="sxs-lookup"><span data-stu-id="4bbde-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="4bbde-110">Če želite več informacij o omejevanju prikaza, [preprečite, da bi se v SharePoint onlineu izognili omejevanju ali blokiranju](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="4bbde-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="4bbde-111">Če imate počasno učinkovitost delovanja s **klasičnim** ali **sodobnim** SharePointovim mestom ali stranjo, uporabite [diagnostično orodje](https://aka.ms/perftool) za analizo strani.</span><span class="sxs-lookup"><span data-stu-id="4bbde-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="4bbde-112">Če še vedno uporabljate splošno počasno učinkovitost delovanja, si oglejte vire na dnu tega članka: [Uvod v prilagajanje učinkovitosti delovanja za SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="4bbde-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  