---
title: Manjka poteka dela ni bilo mogoče aktivirati
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543941"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="5a05a-102">Manjka poteka dela ni bilo mogoče aktivirati</span><span class="sxs-lookup"><span data-stu-id="5a05a-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="5a05a-103">V zbirki mest Microsoft SharePoint, ne morete dodati globalno enkratno uporabo poteka dela (na primer "odobritev - SharePoint 2010") na seznam ali v knjižnico.</span><span class="sxs-lookup"><span data-stu-id="5a05a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="5a05a-104">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="5a05a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="5a05a-105">Odprite spletni koren zbirke mest v SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5a05a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="5a05a-106">Pod **Stran predmetov**, izberite **potek dela**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="5a05a-107">V razdelku **Nova** **poteki dela** traku, izberite **Potek dela za vnovično uporabo**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="5a05a-108">**Ustvarite potek dela za vnovično uporabo** obrazcu, vnesite ime \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="5a05a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="5a05a-109">**Tip platforme**, kliknite **SharePoint 2010 poteka dela**in nato kliknite v **redu**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="5a05a-110">V razdelku **shranjevanje** **potek dela** traku izberite **objavi**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="5a05a-111">V razdelku **upravljanje** **poteka dela** traku izberite **Objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="5a05a-112">V pogovornem oknu potrditve, ki se prikaže, izberite **OK**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="5a05a-113">V spletnem brskalniku, poiščite korenski spletni strani zbirke mest in nato dostopate do **Nastavitev mesta** \> **Funkcij zbirke mest**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="5a05a-114">Nato, zatik zunanja oblika **potekov dela** :</span><span class="sxs-lookup"><span data-stu-id="5a05a-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="5a05a-115">· Če zunanja oblika je *Activated* , kliknite **Deactivate,** in nato kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="5a05a-116">· Če funkcija je *deaktivirani* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="5a05a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="5a05a-117">Za več informacij si oglejte [članek](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="5a05a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

