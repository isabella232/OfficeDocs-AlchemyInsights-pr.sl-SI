---
title: 2010 odobritve poteka dela ni mogoče dodati
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582863"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="0cd84-102">2010 odobritve poteka dela ni mogoče dodati</span><span class="sxs-lookup"><span data-stu-id="0cd84-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="0cd84-103">V zbirki mest Microsoft SharePoint ne morete dodati globalnega poteka dela za enkratno uporabo (na primer» homologacija – SharePoint 2010 «) na seznam ali v knjižnico.</span><span class="sxs-lookup"><span data-stu-id="0cd84-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0cd84-104">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="0cd84-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0cd84-105">Odprite korensko spletno mesto zbirke mest v programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0cd84-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0cd84-106">V razdelku **predmeti mesta**izberite **poteke dela**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0cd84-107">V **novem** odseku traku **potekov dela** izberite **potek dela za večkratno uporabo**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0cd84-108">V obrazcu **Ustvari večkratno uporabo** vnesite ime \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="0cd84-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="0cd84-109">Za **vrsto platforme**kliknite **SharePoint 2010 potek dela**in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="0cd84-110">V odseku **Shrani** v traku **poteka dela** izberite **objavi**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="0cd84-111">V odseku **upravljanje** traku **poteka dela** izberite **objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="0cd84-112">V potrditvenem pogovornem oknu, ki se prikaže, izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="0cd84-113">V spletnem brskalniku poiščite korensko spletno mesto zbirke mest in nato dostopite do **Site Settings** \> **funkcij zbirke**mest za nastavitve mesta.</span><span class="sxs-lookup"><span data-stu-id="0cd84-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="0cd84-114">Preklopite funkcijo **potekov dela** :</span><span class="sxs-lookup"><span data-stu-id="0cd84-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0cd84-115">· Če je funkcija *aktivirana* , kliknite **Deaktiviraj** in nato kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0cd84-116">· Če je funkcija *deaktivirana* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="0cd84-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0cd84-117">Več informacij najdete v naslednjem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="0cd84-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

