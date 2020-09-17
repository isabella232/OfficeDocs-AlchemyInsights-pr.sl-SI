---
title: Ustvarjanje SharePointovega mesta
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806955"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="d0ccd-102">Ustvarjanje SharePointovega mesta</span><span class="sxs-lookup"><span data-stu-id="d0ccd-102">Create a SharePoint site</span></span>

<span data-ttu-id="d0ccd-103">Ustvarite ali upravljajte mesta iz [aktivnih mest](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) v skrbniškem središču za SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="d0ccd-104">Če želite več informacij, glejte [upravljanje spletnih mest v novem skrbniškem središču za SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="d0ccd-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="d0ccd-105">Namigi</span><span class="sxs-lookup"><span data-stu-id="d0ccd-105">Tips:</span></span>

- <span data-ttu-id="d0ccd-106">Mesta **ne morete** ustvariti z istim URL-jem obstoječega mesta.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="d0ccd-107">Če ste izbrisali mesto in želite znova uporabiti spletni naslov, je mogoče, da izbrisano mesto še vedno obstaja v razdelku [izbrisana mesta](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="d0ccd-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="d0ccd-108">Mesto bo treba trajno izbrisati, če želite znova uporabiti spletni naslov.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="d0ccd-109">Če želite v celoti odstraniti mesto z lupino PowerShell, glejte primer» [Odstrani-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) «.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="d0ccd-110">Nekateri uporabniki morda ne bodo mogli ustvariti mesta.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="d0ccd-111">[Glejte upravljanje ustvarjanja mesta v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="d0ccd-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="d0ccd-112">Možno je, da se mesto prikaže, ko **ustvarjate** dlje, kot je bilo pričakovano.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="d0ccd-113">Če je minilo več kot 24 ur, odkar ste prvič videli to težavo, se prijavite v vstopnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="d0ccd-114">V številnih primerih že pripravljamo rešitev.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d0ccd-115">Če želite dokončati rešitev, nam lahko daste vsaj 24 ur.</span><span class="sxs-lookup"><span data-stu-id="d0ccd-115">Please give us at least 24 hours to complete a solution.</span></span>
