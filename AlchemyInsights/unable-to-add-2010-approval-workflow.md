---
title: Ni mogoče dodati potek dela odobritve 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29490393"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="1f3d8-102">Ni mogoče dodati potek dela odobritve 2010</span><span class="sxs-lookup"><span data-stu-id="1f3d8-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="1f3d8-103">V zbirki mest Microsoft SharePoint, ne morete dodati globalno enkratno uporabo poteka dela (na primer "odobritev - SharePoint 2010") na seznam ali v knjižnico.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="1f3d8-104">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="1f3d8-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="1f3d8-105">Odprite spletni koren zbirke mest v SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="1f3d8-106">Pod **Stran predmetov**, izberite **potek dela**.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="1f3d8-107">V razdelku **Nova** **poteki dela** traku, izberite **Potek dela za vnovično uporabo**.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="1f3d8-p101">**Ustvarite potek dela za vnovično uporabo** obrazcu, vnesite ime \*\* *Repair2010* \*\*. **Tip platforme**, kliknite **SharePoint 2010 poteka dela**in nato kliknite v **redu**.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="1f3d8-110">V razdelku **shranjevanje** **potek dela** traku izberite **objavi**.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="1f3d8-p102">V razdelku **upravljanje** **poteka dela** traku izberite **Objavi globalno**. V pogovornem oknu potrditve, ki se prikaže, izberite **OK**.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="1f3d8-p103">V spletnem brskalniku, poiščite korenski spletni strani zbirke mest in nato dostopate do **Nastavitev mesta** \> **Funkcij zbirke mest**. Zatik zunanja oblika **potekov dela** :</span><span class="sxs-lookup"><span data-stu-id="1f3d8-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="1f3d8-115">· Če zunanja oblika je *Activated* , kliknite **Deactivate,** in nato kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="1f3d8-116">· Če funkcija je *deaktivirani* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="1f3d8-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="1f3d8-117">Za več informacij si oglejte [članek](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="1f3d8-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

