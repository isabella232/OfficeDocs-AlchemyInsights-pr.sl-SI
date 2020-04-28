---
title: Obnovitev izbrisanega spletnega mesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: d37fd903c91c8cd6ac6137e815cb253f7edb4494
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912691"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="6d4f0-102">Obnovitev izbrisanega spletnega mesta</span><span class="sxs-lookup"><span data-stu-id="6d4f0-102">Restore a deleted site</span></span>

<span data-ttu-id="6d4f0-103">Ko skrbnik izbriše SharePointovo mesto, ga postavi v zbirko mest recycle bin, kjer je ohranil za 93 dni, preden je trajno izbrisan.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="6d4f0-104">Če želite obnoviti spletno stran:</span><span class="sxs-lookup"><span data-stu-id="6d4f0-104">To restore the site:</span></span>
  
1. <span data-ttu-id="6d4f0-105">V novem skrbniškem središču SharePoint kliknite **koš** na traku.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="6d4f0-106">Potrdite potrditveno polje poleg zbirke mest, ki jo želite obnoviti.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="6d4f0-107">Kliknite **obnovi izbrisane elemente**.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="6d4f0-108">Če želite obnoviti izbrisano mesto za komunikacijo, lahko uporabite novo SharePointovo skrbniško središče.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="6d4f0-109">V nasprotnem primeru morate uporabiti Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="6d4f0-110">Če želite obnoviti spletno mesto, ki pripada skupini Microsoft 365, morate skupino obnoviti v skrbniškem središču za Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-110">To restore a site that belongs to an Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="6d4f0-111">Skupine lahko obnovite 30 dni po izbrisi.</span><span class="sxs-lookup"><span data-stu-id="6d4f0-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

