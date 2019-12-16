---
title: Ustvarjanje SharePointovega mesta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 2611c3ed9cfe78c82c9b123ea26b6fe8f951b458
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049893"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="7f362-102">Ustvarjanje SharePointovega mesta</span><span class="sxs-lookup"><span data-stu-id="7f362-102">Create a SharePoint site</span></span>

<span data-ttu-id="7f362-103">Za informacije o ustvarjanju mesta SharePoint si lahko ogledate naslednje:</span><span class="sxs-lookup"><span data-stu-id="7f362-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="7f362-104">[Upravljajte mesta v novem skrbniškem središču SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Preberite več o možnostih ustvarjanja mest, vključno s tem, kako ustvariti klasično spletno mesto ali mesto ekip, ki ne vključuje skupine Office 365.</span><span class="sxs-lookup"><span data-stu-id="7f362-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="7f362-105">[Ustvarite spletno mesto ekipe v SharePointu](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Naučite se ustvariti spletno mesto skupine.</span><span class="sxs-lookup"><span data-stu-id="7f362-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="7f362-106">[Ustvarite spletno mesto za komunikacijo v SharePointu online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Naučite se ustvariti spletno mesto za komunikacijo.</span><span class="sxs-lookup"><span data-stu-id="7f362-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="7f362-107">[Upravljajte mesta v novem skrbniškem središču SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Naučite se ustvariti klasično spletno mesto ali spletno mesto skupine, ki ne vključuje skupine Office 365.</span><span class="sxs-lookup"><span data-stu-id="7f362-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="7f362-108">**Nasveti:**</span><span class="sxs-lookup"><span data-stu-id="7f362-108">**Tips:**</span></span>
- <span data-ttu-id="7f362-109">Mesta ne morete ustvariti z istim URL-jem obstoječega mesta.</span><span class="sxs-lookup"><span data-stu-id="7f362-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="7f362-110">Če ste izbrisali spletno mesto in želite ponovno uporabiti URL, je možno, da izbrisano mesto še vedno obstaja pod **izbrisanimi spletnimi mesti**.</span><span class="sxs-lookup"><span data-stu-id="7f362-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="7f362-111">Če želite upravljati izbrisana mesta, glejte [brisanje mesta](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="7f362-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="7f362-112">Če želite v celoti odstraniti spletno mesto z lupino PowerShell, glejte primer ukaza» cmdlet « [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="7f362-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="7f362-113">Nekateri uporabniki morda ne bodo mogli ustvariti spletnega mesta.</span><span class="sxs-lookup"><span data-stu-id="7f362-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="7f362-114">Glejte [upravljanje ustvarjanja mest v programu SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7f362-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="7f362-115">Možno je, da je stran videti obtičala pri **ustvarjanju** dlje, kot je bilo pričakovano.</span><span class="sxs-lookup"><span data-stu-id="7f362-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="7f362-116">Če je minilo več kot 24 ur, odkar ste prvič videli to težavo, prosimo, prijavite vozovnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="7f362-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7f362-117">V mnogih primerih že delamo na rešitvi.</span><span class="sxs-lookup"><span data-stu-id="7f362-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7f362-118">Prosimo, dajte nam vsaj 24 ur, da dokončate rešitev.</span><span class="sxs-lookup"><span data-stu-id="7f362-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="7f362-119">Če morate ustvariti novo spletno mesto skupine, ki ne vključuje skupine Office 365,</span><span class="sxs-lookup"><span data-stu-id="7f362-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


