---
title: Potek dela se ne začne
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403759"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="76483-102">Potek dela se ne začne</span><span class="sxs-lookup"><span data-stu-id="76483-102">Workflow is not starting</span></span>

- <span data-ttu-id="76483-103">Poteki dela v strežnikih SharePoint 2010 in SharePoint 2013 se ne začnejo.</span><span class="sxs-lookup"><span data-stu-id="76483-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="76483-104">Če se potek dela ne začne, je morda prišlo do začasne težave storitve, kjer lahko uporabniki pride do začasnih zakasnitev pri poteku dela.</span><span class="sxs-lookup"><span data-stu-id="76483-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="76483-105">Na nadzorni [plošči s stanjem](https://admin.microsoft.com/AdminPortal/Home/servicehealth) storitve preverite, ali je to v vaši organizaciji vplivalo.</span><span class="sxs-lookup"><span data-stu-id="76483-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="76483-106">Če je od prve težave minilo več kot 24 ur, zabeležite vstopnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="76483-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="76483-107">V številnih primerih že delamo na rešitvi.</span><span class="sxs-lookup"><span data-stu-id="76483-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="76483-108">Če želite dokončati rešitev, nam dajte vsaj 24 ur.</span><span class="sxs-lookup"><span data-stu-id="76483-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="76483-109">Poteki dela v programu SharePoint 2010 so na začetku zakasnjeni.</span><span class="sxs-lookup"><span data-stu-id="76483-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="76483-110">Do tega pride, če se potek dela sproži v velikih paketih.</span><span class="sxs-lookup"><span data-stu-id="76483-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="76483-111">(če je na primer dodanih več elementov hkrati).</span><span class="sxs-lookup"><span data-stu-id="76483-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="76483-112">Poteki dela niso načrtovani za izvajanje v realnem času, zato je zakasnitev privzeto vedenje.</span><span class="sxs-lookup"><span data-stu-id="76483-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="76483-113">Če je potek dela zapleten, je zbiranje lahko počasno.</span><span class="sxs-lookup"><span data-stu-id="76483-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="76483-114">Oglejte [si ta](https://support.microsoft.com//kb/3043697) članek.</span><span class="sxs-lookup"><span data-stu-id="76483-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="76483-115">Potek dela bi morali poenostaviti ali ga preoblikovati z vrsto platforme za poteke dela microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="76483-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="76483-116">Če je zgodovina poteka dela več velika, boste morda želeli elemente očistiti ali ustvariti nov seznam zgodovine.</span><span class="sxs-lookup"><span data-stu-id="76483-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="76483-117">Več informacij: [Čiščenje zgodovine poteka dela](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="76483-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="76483-118">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="76483-118">Related topics</span></span>
<span data-ttu-id="76483-119">Ali želite preskusiti Microsoft Flow v SharePoint Onlineu?</span><span class="sxs-lookup"><span data-stu-id="76483-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="76483-120">Create Flow</span><span class="sxs-lookup"><span data-stu-id="76483-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="76483-121">SharePoint in Flow</span><span class="sxs-lookup"><span data-stu-id="76483-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
