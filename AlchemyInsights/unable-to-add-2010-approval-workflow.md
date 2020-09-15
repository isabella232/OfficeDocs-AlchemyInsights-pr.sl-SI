---
title: Poteka dela odobritve za 2010 ni mogoče dodati
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699751"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="159dd-102">Poteka dela odobritve za 2010 ni mogoče dodati</span><span class="sxs-lookup"><span data-stu-id="159dd-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="159dd-103">V zbirki mest Microsoft SharePoint ne morete dodati globalnega poteka dela za vnovično uporabo (na primer» odobritev – SharePoint 2010 «) na seznam ali v knjižnico.</span><span class="sxs-lookup"><span data-stu-id="159dd-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="159dd-104">Če želite odpraviti to težavo, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="159dd-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="159dd-105">Odprite korensko spletno mesto zbirke mest v programu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="159dd-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="159dd-106">V razdelku **predmeti mesta**izberite **poteki dela**.</span><span class="sxs-lookup"><span data-stu-id="159dd-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="159dd-107">V **novem** razdelku traku **poteki dela** izberite» **potek dela «za vnovično uporabo**.</span><span class="sxs-lookup"><span data-stu-id="159dd-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="159dd-108">V obrazcu» **Ustvari ponovno uporabo** «vnesite ime \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="159dd-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="159dd-109">Za **vrsto platforme**kliknite **potek dela za SharePoint 2010**in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="159dd-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="159dd-110">V razdelku» **Shrani** «na traku **poteka dela** izberite **objavi**.</span><span class="sxs-lookup"><span data-stu-id="159dd-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="159dd-111">V razdelku **Upravljaj** na traku **poteka dela** izberite **objavi globalno**.</span><span class="sxs-lookup"><span data-stu-id="159dd-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="159dd-112">V pogovornem oknu za potrditev, ki se prikaže, izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="159dd-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="159dd-113">V spletnem brskalniku poiščite korensko spletno mesto zbirke mest, nato pa kliknite **Site Settings** \> **funkcije zbirke mest**za dostop do mesta.</span><span class="sxs-lookup"><span data-stu-id="159dd-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="159dd-114">Preklop funkcije» **poteki dela** «:</span><span class="sxs-lookup"><span data-stu-id="159dd-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="159dd-115">· Če je funkcija  *aktivirana*  , kliknite **Deaktiviraj** in nato še **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="159dd-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="159dd-116">· Če je funkcija  *deaktivirana*  , kliknite **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="159dd-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="159dd-117">Če želite več informacij, si oglejte ta [članek](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="159dd-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

