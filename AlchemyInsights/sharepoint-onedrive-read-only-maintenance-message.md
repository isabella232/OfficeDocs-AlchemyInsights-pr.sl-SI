---
title: Za sporočilo o vzdrževanju za branje pri poskusu uporabe storitve SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051297"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="7bf7d-102">Za sporočilo o vzdrževanju za branje pri poskusu uporabe storitve SharePoint ali OneDrive</span><span class="sxs-lookup"><span data-stu-id="7bf7d-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="7bf7d-103">Ko poskušate uporabiti SharePoint ali OneDrive za enega od naslednjih scenarijev, lahko uporabniki prejmejo sporočilo **za vzdrževanje samo za branje** .</span><span class="sxs-lookup"><span data-stu-id="7bf7d-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="7bf7d-104">Načrtovana ali aktivna vzdrževalna dejavnost.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="7bf7d-105">Preverite jih tako, da se pomaknete na [center za sporočila](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="7bf7d-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="7bf7d-106">Zelo prednostna, aktivna storitev incident, ki se lahko pojavijo.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="7bf7d-107">Preverite za morebitne Advisories/incidentov, ki jih navigacija do [storitve Health](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7bf7d-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="7bf7d-108">Manjše okrevanje Auto-Healing scenarij, ki bi se lahko dogajalo zaradi kakršnih koli nepričakovanih dogodkov na strežnikih, ki bi lahko trajala manj kot 30 min ali tako.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="7bf7d-109">Ni sporočila center ali Service Health delovnih mest za te manjše izterjave, vendar bi morali biti nazaj na normalno zelo kmalu.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="7bf7d-110">Ob zelo redkih priložnostih smo opazili, da je eden od treh zgoraj naštetih scenarijev je bil vzrok, in storitev je bila obnovljena, vendar uporabniki brskalnika predpomnilnik ni bil očiščen.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="7bf7d-111">Pred navigacijo do spletnega mesta poskusite počistiti predpomnilnik brskalnika.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="7bf7d-112">V brskalniku Microsoft Edge izberite **Nastavitve**, nato pa izberite **zasebnost in varnost**.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="7bf7d-113">Pod možnostjo **Izbriši brskanje**izberite izberite **, kaj želite počistiti**.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="7bf7d-114">Izberite **piškotki in shranjeni podatki spletnega mesta**ter izberite **Počisti**.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="7bf7d-115">Ti koraki se lahko razlikujejo pri uporabi drugih brskalnikov, kot sta Mozilla Firefox ali Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="7bf7d-116">Druga možnost bi bila, da odprete SharePointovo spletno mesto ali OneDrive v novem oknu InPrivate.</span><span class="sxs-lookup"><span data-stu-id="7bf7d-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>