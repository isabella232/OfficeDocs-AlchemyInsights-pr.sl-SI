---
title: Trajno brisanje spletnega mesta v SharePointu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955237"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="7e729-102">Trajno brisanje spletnega mesta v SharePointu</span><span class="sxs-lookup"><span data-stu-id="7e729-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="7e729-103">Če želite znova uporabiti URL izbrisanega spletnega mesta (za vnovično ustvarjanje mesta) ali trajno izbrisati spletno mesto, ker ga ne uporabljate več, lahko uporabite možnost **Trajno izbriši** v novem Skrbniškem središču SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e729-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="7e729-104">Pojdite na [stran z izbrisanimi spletnimi mesti v novem Skrbniškem središču SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) ter se vpišite z računom s skrbniškimi dovoljenji za organizacijo.</span><span class="sxs-lookup"><span data-stu-id="7e729-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="7e729-105">V levem stolpcu izberite spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="7e729-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="7e729-106">Kliknite **Trajno izbriši**.</span><span class="sxs-lookup"><span data-stu-id="7e729-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="7e729-107">**Opomba**: spletnih mest, povezanih s skupinami, ni mogoče trajno izbrisati v novem Skrbniškem središču SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7e729-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="7e729-108">Namesto tega uporabite ukaz [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="7e729-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="7e729-109">Za več informacij glejte [Trajno brisanje spletnega mesta](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="7e729-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
