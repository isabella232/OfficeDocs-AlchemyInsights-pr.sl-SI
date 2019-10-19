---
title: Manjkajoč potek dela ni uspel aktivirati
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753812"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="8e34a-102">Manjkajoč potek dela ni uspel aktivirati</span><span class="sxs-lookup"><span data-stu-id="8e34a-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="8e34a-103">V zbirki mest Microsoft SharePoint ne morete dodati globalnega poteka dela za enkratno uporabo (na primer» homologacija – SharePoint 2010 «) na seznam ali v knjižnico.</span><span class="sxs-lookup"><span data-stu-id="8e34a-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="8e34a-104">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="8e34a-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="8e34a-105">Odprite korensko spletno mesto zbirke mest v programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="8e34a-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="8e34a-106">V razdelku **predmeti mesta**izberite **poteke dela**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="8e34a-107">V **novem** odseku traku **potekov dela** izberite **potek dela za večkratno uporabo**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="8e34a-108">V obrazcu **Ustvari večkratno uporabo** vnesite ime \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="8e34a-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="8e34a-109">Za **vrsto platforme**kliknite **SharePoint 2010 potek dela**in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="8e34a-110">V odseku **Shrani** v traku **poteka dela** izberite **objavi**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="8e34a-111">V odseku **upravljanje** traku **poteka dela** izberite **objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="8e34a-112">V potrditvenem pogovornem oknu, ki se prikaže, izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="8e34a-113">V spletnem brskalniku poiščite korensko spletno mesto zbirke mest in nato dostopite do **funkcij zbirke**mest za **Nastavitve** \> mesta.</span><span class="sxs-lookup"><span data-stu-id="8e34a-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="8e34a-114">Nato preklopite funkcijo **potekov dela** :</span><span class="sxs-lookup"><span data-stu-id="8e34a-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="8e34a-115">· Če je funkcija *aktivirana* , kliknite **Deaktiviraj** in nato kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="8e34a-116">· Če je funkcija *deaktivirana* , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="8e34a-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="8e34a-117">Več informacij najdete v naslednjem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="8e34a-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

