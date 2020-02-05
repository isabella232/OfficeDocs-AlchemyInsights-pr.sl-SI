---
title: Ustvarjanje SharePointovega mesta
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770871"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="fbdc9-102">Ustvarjanje SharePointovega mesta</span><span class="sxs-lookup"><span data-stu-id="fbdc9-102">Create a SharePoint site</span></span>

<span data-ttu-id="fbdc9-103">Ustvarite ali upravljajte mesta iz [aktivnih mest](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) v SharePointovem skrbniškem središču.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="fbdc9-104">Če želite več informacij, glejte [upravljanje spletnih mest v novem skrbniškem središču SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="fbdc9-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="fbdc9-105">Nasveti:</span><span class="sxs-lookup"><span data-stu-id="fbdc9-105">Tips:</span></span>

- <span data-ttu-id="fbdc9-106">Mesta **ni mogoče** ustvariti z ISTIM URL-jem obstoječega mesta.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="fbdc9-107">Če ste izbrisali spletno mesto in želite ponovno uporabiti URL, je možno, da izbrisano mesto še vedno obstaja pod [izbrisanimi spletnimi mesti](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="fbdc9-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="fbdc9-108">Stran bo treba trajno izbrisati, da ponovno uporabite URL.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="fbdc9-109">Če želite v celoti odstraniti spletno mesto z lupino PowerShell, glejte primer ukaza» cmdlet « [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="fbdc9-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="fbdc9-110">Nekateri uporabniki morda ne bodo mogli ustvariti spletnega mesta.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="fbdc9-111">[Glejte upravljanje ustvarjanja mest v programu SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="fbdc9-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="fbdc9-112">Možno je, da je stran videti obtičala pri **ustvarjanju** dlje, kot je bilo pričakovano.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="fbdc9-113">Če je minilo več kot 24 ur, odkar ste prvič videli to težavo, prosimo, prijavite vozovnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="fbdc9-114">V mnogih primerih že delamo na rešitvi.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="fbdc9-115">Prosimo, dajte nam vsaj 24 ur, da dokončate rešitev.</span><span class="sxs-lookup"><span data-stu-id="fbdc9-115">Please give us at least 24 hours to complete a solution.</span></span>
