---
title: Uvod v SharePoint online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 4c0220dd2535a1ef41aeef99e2bfc3fe28bac03a
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751688"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="9bf65-102">Poteki dela v SharePointu</span><span class="sxs-lookup"><span data-stu-id="9bf65-102">Workflows in SharePoint</span></span>

<span data-ttu-id="9bf65-103">Če SharePointovi poteki dela ne pošiljajo e-poštnih sporočil, je morda vaša organizacija naletela na omejitve pošiljatelja Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9bf65-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="9bf65-104">Sporočilo o napaki» potek dela je Prekineno «se lahko pojavi, če imate enega od teh elementov:</span><span class="sxs-lookup"><span data-stu-id="9bf65-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="9bf65-105">V programu SharePoint online poteka potek dela, ki uporablja vrsto platforme za potek dela SharePoint 2010 ali SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="9bf65-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="9bf65-106">Potek dela je konfiguriran tako, da pošlje e-poštno sporočilo po meri več kot 200 uporabnikom naenkrat, več kot 10.000 prejemnikov na dan ali več kot 30 sporočil na minuto.</span><span class="sxs-lookup"><span data-stu-id="9bf65-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="9bf65-107">Ko zaženete potek dela, e-poštno sporočilo ni poslano in opazite sporočilo o napaki, je notranje stanje nastavljeno na začasno ali ne more poslati prejemniku.</span><span class="sxs-lookup"><span data-stu-id="9bf65-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="9bf65-108">Za več informacij glejte naslednji [članek](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="9bf65-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

