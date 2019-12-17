---
title: Težave z učinkovitostjo delovanja-SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068434"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="2b8c9-102">SharePoint ali OneDrive je počasen, nedostopen ali ni na voljo za več uporabnikov</span><span class="sxs-lookup"><span data-stu-id="2b8c9-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="2b8c9-103">SharePoint ali OneDrive je lahko počasen, nedosegljiv ali na voljo ali pa lahko prikaže storitev, ki ni na voljo, ali 503 napak iz več razlogov:</span><span class="sxs-lookup"><span data-stu-id="2b8c9-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="2b8c9-104">Če je vaše spletno mesto SharePoint ali OneDrive počasno ali Zakasnjeno za več uporabnikov, lahko pride do začasne težave s storitvijo, kjer uporabniki pri dostopu do SharePointovih mest ali vsebine v storitvi OneDrive izkusijo prekinjene zamude ali napake pri krmarjenju.</span><span class="sxs-lookup"><span data-stu-id="2b8c9-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="2b8c9-105">Če želite preveriti, ali je vaša organizacija vplivala, preverite [nadzorno ploščo storitve](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="2b8c9-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="2b8c9-106">Uporabnik maj sprejemati a *503 pomočnik je zaposlen* zmota čas poskus v pluti v SharePoint ali OneDrive položaj.</span><span class="sxs-lookup"><span data-stu-id="2b8c9-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="2b8c9-107">To napako lahko povzroči zadavljenje znotraj storitve SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2b8c9-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="2b8c9-108">SharePoint online uporablja zadaviti za ohranjanje optimalne učinkovitosti in zanesljivosti storitve SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="2b8c9-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="2b8c9-109">Throttling omejuje število uporabniških dejanj ali sočasnih klicev (po skriptu ali kodi), da se prepreči prekomerna uporaba virov.</span><span class="sxs-lookup"><span data-stu-id="2b8c9-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="2b8c9-110">Za več informacij o zadaviti glej, [ne pridobivanje zadaviti ali blokiran v SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="2b8c9-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="2b8c9-111">Če doživite počasno delovanje s **klasičnim** ali **modernim** SharePointovim mestom ali stranjo, uporabite [diagnostično orodje](https://aka.ms/perftool) za analizo strani.</span><span class="sxs-lookup"><span data-stu-id="2b8c9-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="2b8c9-112">Če še vedno doživite splošno počasno delovanje, preglejte vire na dnu tega članka: [Uvod v tuning učinkovitosti za SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="2b8c9-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  