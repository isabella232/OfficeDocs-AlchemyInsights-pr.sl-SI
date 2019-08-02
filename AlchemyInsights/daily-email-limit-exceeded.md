---
title: Dnevni email omejitev prekoračena. Potek dela je prekinjena.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059654"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="6baca-103">Dnevni email prekoračena.</span><span class="sxs-lookup"><span data-stu-id="6baca-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="6baca-104">Potek dela je prekinjena.</span><span class="sxs-lookup"><span data-stu-id="6baca-104">Workflow is suspended.</span></span>

<span data-ttu-id="6baca-105">To napako lahko prejel v naslednjih primerih:</span><span class="sxs-lookup"><span data-stu-id="6baca-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="6baca-106">Imate potek dela v SharePoint Online, ki uporablja SharePoint 2010 ali tip platforme SharePoint 2013 poteka dela.</span><span class="sxs-lookup"><span data-stu-id="6baca-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="6baca-107">Potek dela je nastavljen tako, da po meri email sporočilo poslati več kot 200 uporabnikov naenkrat, več kot 10.000 prejemniki na dan ali več kot 30 sporočil na minuto.</span><span class="sxs-lookup"><span data-stu-id="6baca-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="6baca-108">Ko zaženete potek dela, e-poštno sporočilo ni poslano, in boste opazili naslednje težave:</span><span class="sxs-lookup"><span data-stu-id="6baca-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="6baca-109">Za potek dela z uporabo tip platforme SharePoint 2013, poiščite stran **Stanja poteka dela** .</span><span class="sxs-lookup"><span data-stu-id="6baca-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="6baca-110">«Na strani» stanje poteka dela« **Notranje stanje** nastavljeno na **Started**in oblaček z informacijami prikaže **ni mogoče poslati prejemniku**.</span><span class="sxs-lookup"><span data-stu-id="6baca-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="6baca-111">Tej težavi, konfigurirajte potek dela za pošiljanje e-poštnih sporočil ne preseže [Exchange Online pošiljatelj omejitve](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="6baca-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="6baca-112">Na primer, uporabite premor v poteku dela, spodbuda email v Office 365 skupine, skupine prejemnikov ali pošte omogočena varnostne skupine ali Pošlji sporočilo manj kot 200 prejemnikom naenkrat.</span><span class="sxs-lookup"><span data-stu-id="6baca-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="6baca-113">Če želite več informacij, glejte ta [članek](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="6baca-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="6baca-114">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="6baca-114">Related topics</span></span>
- [<span data-ttu-id="6baca-115">Ustvari tok</span><span class="sxs-lookup"><span data-stu-id="6baca-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="6baca-116">SharePoint in pretok</span><span class="sxs-lookup"><span data-stu-id="6baca-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 