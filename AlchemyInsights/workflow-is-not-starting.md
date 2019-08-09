---
title: Potek dela se ne začenja
ms.author: efrene
author: efrene
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270796"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="02c0b-102">Potek dela se ne začenja</span><span class="sxs-lookup"><span data-stu-id="02c0b-102">Workflow is not starting</span></span>

- <span data-ttu-id="02c0b-103">SharePoint 2010 in SharePoint 2013 poteki dela ne začenjajo.</span><span class="sxs-lookup"><span data-stu-id="02c0b-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="02c0b-104">Če vaš potek dela ne zažene, lahko pride do začasnih storitev vprašanje če uporabnik pride do občasne zakasnitve z napredkom poteka dela.</span><span class="sxs-lookup"><span data-stu-id="02c0b-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="02c0b-105">Preverite [Nadzorna plošča storitev za zdravje](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , da vidim, če vaša organizacija je vplivala.</span><span class="sxs-lookup"><span data-stu-id="02c0b-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="02c0b-106">Če več kot 24 ur je minilo, odkar je prvič videl to vprašanje, se prijavite podporo vozovnice.</span><span class="sxs-lookup"><span data-stu-id="02c0b-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="02c0b-107">V mnogih primerih, že delamo na rešitev.</span><span class="sxs-lookup"><span data-stu-id="02c0b-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="02c0b-108">Prosimo, da nam vsaj 24 ur za dokončanje rešitev.</span><span class="sxs-lookup"><span data-stu-id="02c0b-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="02c0b-109">Poteki dela za SharePoint 2010 odloži na začetek.</span><span class="sxs-lookup"><span data-stu-id="02c0b-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="02c0b-110">To se zgodi, če je potek dela sprožen v velikih serijah.</span><span class="sxs-lookup"><span data-stu-id="02c0b-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="02c0b-111">(na primer, ko več so dodani elementi naenkrat).</span><span class="sxs-lookup"><span data-stu-id="02c0b-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="02c0b-112">Poteki dela so niso konstruirani za vožnjo v realnem času, tako da zamude pri načrtovanju vedenje.</span><span class="sxs-lookup"><span data-stu-id="02c0b-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="02c0b-113">Če poteka kompleksna Extensible predmet označevalni jezik (XMOL), lahko počasno urejanje.</span><span class="sxs-lookup"><span data-stu-id="02c0b-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="02c0b-114">Preverite [ta](https://support.microsoft.com/en-us/kb/3043697) članek.</span><span class="sxs-lookup"><span data-stu-id="02c0b-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="02c0b-115">Naj poenostavaiti workflow ali preoblikovanje z tip platforme Microsoft SharePoint 2013 poteka dela.</span><span class="sxs-lookup"><span data-stu-id="02c0b-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="02c0b-116">Če zgodovine poteka dela je zrasel velik, morda boste želeli Počisti elemente ali ustvarite nov seznam zgodovine.</span><span class="sxs-lookup"><span data-stu-id="02c0b-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="02c0b-117">Več informacij: [Počisti zgodovino poteka dela](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="02c0b-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="02c0b-118">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="02c0b-118">Related topics</span></span>
<span data-ttu-id="02c0b-119">Želite poskusiti Microsoft Flow v SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="02c0b-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="02c0b-120">Ustvari tok</span><span class="sxs-lookup"><span data-stu-id="02c0b-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="02c0b-121">SharePoint in pretok</span><span class="sxs-lookup"><span data-stu-id="02c0b-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


