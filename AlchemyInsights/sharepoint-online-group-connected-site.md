---
title: Dodajanje skupine na SharePointovo mesto
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582827"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="f5af3-102">Težave pri ustvarjanju skupine, povezane z mestom v SharePointu</span><span class="sxs-lookup"><span data-stu-id="f5af3-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="f5af3-103">Nekatera pogosta vprašanja, ki so se pojavile pri ustvarjanju ali vnovični vzpostavitvi povezanega spletnega mesta skupine.</span><span class="sxs-lookup"><span data-stu-id="f5af3-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="f5af3-104">Če ste izbrisali skupino in njeno povezano spletno mesto in želite ustvariti drugo spletno mesto z istim URL-jem, boste morali trajno odstraniti prejšnje mesto.</span><span class="sxs-lookup"><span data-stu-id="f5af3-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="f5af3-105">Travnato gričevje [spo uprava skorja](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="f5af3-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="f5af3-106">Če želite več informacij o tem, kako začeti z lupino PowerShell, glejte [Uvod v SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="f5af3-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="f5af3-107">Odstranite stran iz izbrisanih mest z ukazom» cmdlet « [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f5af3-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="f5af3-108">PowerShell je treba trajno izbrisati skupine mest.</span><span class="sxs-lookup"><span data-stu-id="f5af3-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="f5af3-109">Če ustvarjate skupinsko povezano mesto in prejmete opozorilo: **druga skupina z istim vzdevkom že obstaja**, preverite obstoječe skupine iz [skrbniškega središča Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="f5af3-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="f5af3-110">Če želite odpraviti težavo, izbrišite obstoječo skupino, če je ni več potrebno ali ustvarite mesto z drugim dodeljenim vzdevkom.</span><span class="sxs-lookup"><span data-stu-id="f5af3-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="f5af3-111">Obstajajo različni načini za ustvarjanje in uporabo sodobnih skupin s SharePointom.</span><span class="sxs-lookup"><span data-stu-id="f5af3-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="f5af3-112">Obstoječa mesta lahko povežete s skupino Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f5af3-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="f5af3-113">Če želite več informacij, glejte [povezovanje skupine Microsoft 365 s SharePointovim uporabniškim vmesnikom](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="f5af3-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="f5af3-114">Če želite ustvariti povezano spletno mesto skupine Microsoft 365, morate ustvariti [spletno mesto skupine](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="f5af3-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
