---
title: Potek dela se ne zažene
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794783"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="54130-102">Potek dela se ne zažene</span><span class="sxs-lookup"><span data-stu-id="54130-102">Workflow is not starting</span></span>

- <span data-ttu-id="54130-103">Poteki dela programa SharePoint 2010 in SharePoint 2013 se ne zaženeta.</span><span class="sxs-lookup"><span data-stu-id="54130-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="54130-104">Če se potek dela ne zažene, je morda prišlo do začasne težave s storitvijo, kjer lahko uporabniki občasno zadržijo zamude pri napredovanju poteka dela.</span><span class="sxs-lookup"><span data-stu-id="54130-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="54130-105">Preverite, ali je [Nadzorna plošča za zdravstveno stanje na voljo](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , če želite preveriti, ali je vaša organizacija vplivala nanje.</span><span class="sxs-lookup"><span data-stu-id="54130-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="54130-106">Če je minilo več kot 24 ur, odkar ste prvič videli to težavo, se prijavite v vstopnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="54130-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="54130-107">V številnih primerih že pripravljamo rešitev.</span><span class="sxs-lookup"><span data-stu-id="54130-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="54130-108">Če želite dokončati rešitev, nam lahko daste vsaj 24 ur.</span><span class="sxs-lookup"><span data-stu-id="54130-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="54130-109">Poteki dela programa SharePoint 2010 so zakasnjeni ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="54130-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="54130-110">Do tega pride, če je potek dela sprožen v velikih paketih.</span><span class="sxs-lookup"><span data-stu-id="54130-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="54130-111">(na primer, ko je več elementov dodanih hkrati).</span><span class="sxs-lookup"><span data-stu-id="54130-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="54130-112">Poteki dela niso zasnovani za zagon v realnem času, tako da je zamuda vedenje po načrtovanju.</span><span class="sxs-lookup"><span data-stu-id="54130-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="54130-113">Če gre za potek dela, je zapleteni jezik označevalnih predmetov (XMOL), urejanje je lahko počasno.</span><span class="sxs-lookup"><span data-stu-id="54130-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="54130-114">Oglejte si [ta](https://support.microsoft.com//kb/3043697) članek.</span><span class="sxs-lookup"><span data-stu-id="54130-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="54130-115">Potek dela lahko poenostavite ali ga preoblikujete z vrsto platforme za potek dela programa Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="54130-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="54130-116">Če je zgodovina poteka dela velika, boste morda želeli izbrisati elemente ali ustvariti nov seznam zgodovine.</span><span class="sxs-lookup"><span data-stu-id="54130-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="54130-117">Več informacij: čiščenje [zgodovine poteka dela](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="54130-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="54130-118">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="54130-118">Related topics</span></span>
<span data-ttu-id="54130-119">Ali želite preskusiti Microsoft Flow v storitvi SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="54130-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="54130-120">Ustvarjanje toka</span><span class="sxs-lookup"><span data-stu-id="54130-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="54130-121">SharePoint in Flow</span><span class="sxs-lookup"><span data-stu-id="54130-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


