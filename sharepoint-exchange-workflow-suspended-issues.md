---
title: Uvod v SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 9a8d72a01ed35794fcab370b48bbb189663d3396
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34718762"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="8db0f-102">Poteke dela v SharePointu</span><span class="sxs-lookup"><span data-stu-id="8db0f-102">Workflows in SharePoint</span></span>

<p><span data-ttu-id="8db0f-103">Če SharePoint poteki dela ne pošiljate e-pošto, vaše organizacije so se pojavile meje Exchange Online pošiljatelja.&nbsp;</span><span class="sxs-lookup"><span data-stu-id="8db0f-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.&nbsp;</span></span></p> <p><span data-ttu-id="8db0f-104">"Potek dela je prekinjena" sporočilo o napaki pride, če imate eno od naslednjih postavk:</span><span class="sxs-lookup"><span data-stu-id="8db0f-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span></p> <ul> <li><span data-ttu-id="8db0f-105">Imate potek dela v SharePoint Online, ki uporablja SharePoint 2010 ali tip platforme SharePoint 2013 poteka dela.</span><span class="sxs-lookup"><span data-stu-id="8db0f-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span></li> <li><span data-ttu-id="8db0f-106">Potek dela je nastavljen tako, da po meri email sporočilo poslati več kot 200 uporabnikov naenkrat, več kot 10.000 prejemniki na dan ali več kot 30 sporočil na minuto.</span><span class="sxs-lookup"><span data-stu-id="8db0f-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span></li> <li><span data-ttu-id="8db0f-107">Ko zaženete potek dela, e-poštno sporočilo ni poslano, in boste opazili sporočilo o napaki, se prikaže <strong>notranje stanje nastavljeno na prekinjena</strong> ali <strong>ni mogoče poslati prejemniku</strong> .</span><span class="sxs-lookup"><span data-stu-id="8db0f-107">When you run the workflow, the email message isn't sent, and you notice the error message, <strong>Internal Status is set to Suspended</strong> or <strong>Unable to send to a recipient</strong> is displayed.</span></span></li> </ul> <p><span data-ttu-id="8db0f-108">Če želite več informacij, si oglejte <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">članek</a>.</span><span class="sxs-lookup"><span data-stu-id="8db0f-108">For more information, please refer to the following <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">article</a>.</span></span></p>

