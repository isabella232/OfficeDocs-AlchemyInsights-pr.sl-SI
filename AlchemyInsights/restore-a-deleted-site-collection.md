---
title: Obnovitev izbrisanega mest
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 22fb513771abc1a604a347204bac268771cb9e37
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29940012"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="f121c-102">Obnovitev izbrisanega mest</span><span class="sxs-lookup"><span data-stu-id="f121c-102">Restore a deleted site collection</span></span>

<span data-ttu-id="f121c-p101">Ko admin izbriše zbirko klasičnih mest, se nahaja v zbirki mest koš, kjer se hrani za 93 dni preden pa se trajno izbriše. Če želite obnoviti zbirko mest:</span><span class="sxs-lookup"><span data-stu-id="f121c-p101">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted. To restore the site collection:</span></span>
  
1. <span data-ttu-id="f121c-105">V klasičnih SharePoint admin center, na traku kliknite **Koš** .</span><span class="sxs-lookup"><span data-stu-id="f121c-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="f121c-106">Izberite potrditveno polje ob zbirki spletnih mest, ki jo želite obnoviti.</span><span class="sxs-lookup"><span data-stu-id="f121c-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="f121c-107">Kliknite **obnovi izbrisane elemente**.</span><span class="sxs-lookup"><span data-stu-id="f121c-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="f121c-p102">Da obnovite izbrisano sporočilo, lahko uporabite novo SharePoint admin center predogled. V nasprotnem primeru morate uporabiti PowerShell. Za obnovitev mesta, ki spada v skupino Office 365, morate obnoviti skupini v skrbniškem središču za izmenjavo. Skupine je mogoče obnoviti za 30 dni potem, ko so izbrisana.</span><span class="sxs-lookup"><span data-stu-id="f121c-p102">To restore a deleted communication site, you can use the new SharePoint admin center preview. Otherwise, you need to use PowerShell. To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center. Groups can be restored for 30 days after they're deleted.</span></span>
  

