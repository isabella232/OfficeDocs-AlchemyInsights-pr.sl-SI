---
title: Uvod v SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700723"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="165b1-102">Poteki dela v SharePointu</span><span class="sxs-lookup"><span data-stu-id="165b1-102">Workflows in SharePoint</span></span>

<span data-ttu-id="165b1-103">Če SharePointovi poteki dela ne pošiljajo e-poštnih sporočil, je vaša organizacija morda naletela na omejitve pošiljatelja za Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="165b1-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="165b1-104">Sporočilo o napaki» potek dela je začasno ustavljeno «lahko pride, če imate enega od teh elementov:</span><span class="sxs-lookup"><span data-stu-id="165b1-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="165b1-105">V storitvi SharePoint online imate potek dela, ki uporablja vrsto platforme za potek dela za SharePoint 2010 ali SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="165b1-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="165b1-106">Potek dela je konfiguriran za pošiljanje e-poštnega sporočila po meri več kot 200 uporabnikom hkrati, več kot 10.000 prejemnikov na dan ali več kot 30 sporočil na minuto.</span><span class="sxs-lookup"><span data-stu-id="165b1-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="165b1-107">Ko zaženete potek dela, se e-poštno sporočilo ne pošlje in opazite sporočilo o napaki, da je notranje stanje nastavljeno na začasno prekinjeno ali ne more poslati prejemniku.</span><span class="sxs-lookup"><span data-stu-id="165b1-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="165b1-108">Če želite več informacij, si oglejte ta [članek](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span><span class="sxs-lookup"><span data-stu-id="165b1-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

