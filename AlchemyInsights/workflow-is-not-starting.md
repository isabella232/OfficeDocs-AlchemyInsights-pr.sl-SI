---
title: Potek dela se ne začenja
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049353"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="91e28-102">Potek dela se ne začenja</span><span class="sxs-lookup"><span data-stu-id="91e28-102">Workflow is not starting</span></span>

- <span data-ttu-id="91e28-103">Poteki dela SharePoint 2010 in SharePoint 2013 se ne začenjajo.</span><span class="sxs-lookup"><span data-stu-id="91e28-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="91e28-104">Če se potek dela ne začne, lahko pride do začasne težave s storitvijo, kjer lahko uporabniki občasno povzročijo zamude pri poteku dela.</span><span class="sxs-lookup"><span data-stu-id="91e28-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="91e28-105">Če želite preveriti, ali je vaša organizacija vplivala, preverite [Nadzorna plošča storitve](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) .</span><span class="sxs-lookup"><span data-stu-id="91e28-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="91e28-106">Če je minilo več kot 24 ur, odkar ste prvič videli to težavo, prosimo, prijavite vozovnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="91e28-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="91e28-107">V mnogih primerih že delamo na rešitvi.</span><span class="sxs-lookup"><span data-stu-id="91e28-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="91e28-108">Prosimo, dajte nam vsaj 24 ur, da dokončate rešitev.</span><span class="sxs-lookup"><span data-stu-id="91e28-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="91e28-109">Poteki dela SharePoint 2010 so bili ob zagonu zakasnjeni.</span><span class="sxs-lookup"><span data-stu-id="91e28-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="91e28-110">To se zgodi, če je potek dela sprožen v velikih serijah.</span><span class="sxs-lookup"><span data-stu-id="91e28-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="91e28-111">(na primer, ko je več elementov dodanih naenkrat).</span><span class="sxs-lookup"><span data-stu-id="91e28-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="91e28-112">Poteki dela niso zasnovani za zagon v realnem času, zato je zakasnitev po-design vedenje.</span><span class="sxs-lookup"><span data-stu-id="91e28-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="91e28-113">Če je potek dela kompleksen Extensible Object Markup Language (XMOL), lahko kompilacija je počasna.</span><span class="sxs-lookup"><span data-stu-id="91e28-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="91e28-114">Preverite [ta](https://support.microsoft.com//kb/3043697) članek.</span><span class="sxs-lookup"><span data-stu-id="91e28-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="91e28-115">Potek dela ali preoblikovanje je treba poenostaviti z vrsto platforme Microsoft SharePoint 2013 Workflow.</span><span class="sxs-lookup"><span data-stu-id="91e28-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="91e28-116">Če se je zgodovina poteka dela povečala, boste morda želeli Počisti elemente ali ustvariti nov seznam zgodovine.</span><span class="sxs-lookup"><span data-stu-id="91e28-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="91e28-117">Več informacij: [purge zgodovina poteka dela](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="91e28-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="91e28-118">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="91e28-118">Related topics</span></span>
<span data-ttu-id="91e28-119">Želite poskusiti Microsoft Flow v SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="91e28-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="91e28-120">Ustvari potek</span><span class="sxs-lookup"><span data-stu-id="91e28-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="91e28-121">SharePoint in Flow</span><span class="sxs-lookup"><span data-stu-id="91e28-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


