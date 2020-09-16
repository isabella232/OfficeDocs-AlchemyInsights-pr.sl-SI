---
title: Omejitev dnevne pošte je presežena. Potek dela je prekinjen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731579"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="26a2b-103">Omejitev dnevne pošte je presežena.</span><span class="sxs-lookup"><span data-stu-id="26a2b-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="26a2b-104">Potek dela je prekinjen.</span><span class="sxs-lookup"><span data-stu-id="26a2b-104">Workflow is suspended.</span></span>

<span data-ttu-id="26a2b-105">To napako lahko prejmete v teh primerih:</span><span class="sxs-lookup"><span data-stu-id="26a2b-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="26a2b-106">V storitvi SharePoint online imate potek dela, ki uporablja vrsto platforme za potek dela za SharePoint 2010 ali SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="26a2b-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="26a2b-107">Potek dela je konfiguriran za pošiljanje e-poštnega sporočila po meri več kot 200 uporabnikom hkrati, več kot 10.000 prejemnikov na dan ali več kot 30 sporočil na minuto.</span><span class="sxs-lookup"><span data-stu-id="26a2b-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="26a2b-108">Ko zaženete potek dela, se e-poštno sporočilo ne pošlje in opazite to težavo:</span><span class="sxs-lookup"><span data-stu-id="26a2b-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="26a2b-109">Za potek dela z vrsto platforme SharePoint 2013 se pomaknite do strani **stanje poteka dela** .</span><span class="sxs-lookup"><span data-stu-id="26a2b-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="26a2b-110">Na strani stanja poteka dela je **stanje notranjega stanja** nastavljeno na **začetek**, oblaček z informacijami pa **ne more poslati prejemniku**.</span><span class="sxs-lookup"><span data-stu-id="26a2b-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="26a2b-111">Če se želite izogniti tej težavi, konfigurirajte potek dela za pošiljanje e-poštnih sporočil, ne da bi presegli [omejitve pošiljatelja Exchange Onlinea](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="26a2b-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="26a2b-112">Uporabite na primer premor v poteku dela, pošljite e-pošto v skupino Microsoft 365, skupino prejemnikov ali varnostno skupino z omogočeno pošto ali pa pošljite sporočilo manj kot 200 prejemnikom hkrati.</span><span class="sxs-lookup"><span data-stu-id="26a2b-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="26a2b-113">Če želite več informacij, si oglejte ta [članek](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="26a2b-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="26a2b-114">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="26a2b-114">Related topics</span></span>
- [<span data-ttu-id="26a2b-115">Ustvarjanje toka</span><span class="sxs-lookup"><span data-stu-id="26a2b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="26a2b-116">SharePoint in Flow</span><span class="sxs-lookup"><span data-stu-id="26a2b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 