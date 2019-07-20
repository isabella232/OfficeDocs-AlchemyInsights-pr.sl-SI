---
title: Ustvarite SharePointovo mesto
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802982"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="c6b26-102">Ustvarite SharePointovo mesto</span><span class="sxs-lookup"><span data-stu-id="c6b26-102">Create a SharePoint site</span></span>

<span data-ttu-id="c6b26-103">Ogledate si lahko naslednje informacije o ustvarjanje SharePoint mesta:</span><span class="sxs-lookup"><span data-stu-id="c6b26-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="c6b26-104">[Upravljanje mesta v centru nove SharePoint admin](https://docs.microsoft.com/sharepoint/manage-site-creation): več o možnostih oblikovanja mesta, ustvarjanju klasična stran ali stran ekipe, ki ne vključuje skupino Office 365.</span><span class="sxs-lookup"><span data-stu-id="c6b26-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="c6b26-105">[Ustvari mesta skupine SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Naučite se ustvariti mesto ekipa.</span><span class="sxs-lookup"><span data-stu-id="c6b26-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="c6b26-106">[Ustvari sporočilo mestu SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Naučite se, kako ustvariti spletno stran komunikacije.</span><span class="sxs-lookup"><span data-stu-id="c6b26-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="c6b26-107">[Upravljanje mesta v centru nove SharePoint admin](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Naučite se ustvariti klasična stran ali mesto ekipe, ki ne vključuje skupino Office 365.</span><span class="sxs-lookup"><span data-stu-id="c6b26-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Nasveti]
> - <span data-ttu-id="c6b26-109">Mesta ni mogoče ustvariti z istega URL obstoječega mesta.</span><span class="sxs-lookup"><span data-stu-id="c6b26-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="c6b26-110">Če izbrisati mesto in se želijo ponovno uporabiti URL, je mogoče izbrisati mesto še vedno obstaja pod **Izbrisano mesta**.</span><span class="sxs-lookup"><span data-stu-id="c6b26-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="c6b26-111">Za upravljanje izbrisane strani glej, [izbrišite mesto](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="c6b26-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="c6b26-112">V čisto premestitev stran z Powershell, glej primer [Odstrani-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet.</span><span class="sxs-lookup"><span data-stu-id="c6b26-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="c6b26-113">Nekateri uporabniki lahko ne morete ustvariti spletno stran.</span><span class="sxs-lookup"><span data-stu-id="c6b26-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="c6b26-114">Glejte [upravljanje ustvarjanje mesta v SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="c6b26-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="c6b26-115">Je mogoče, stran se prikaže zaljubljen v **Ustvarjanje** dlje kot pričakovano.</span><span class="sxs-lookup"><span data-stu-id="c6b26-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="c6b26-116">Če več kot 24 ur je minilo, odkar je prvič videl to vprašanje, se prijavite podporo vozovnice.</span><span class="sxs-lookup"><span data-stu-id="c6b26-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="c6b26-117">V mnogih primerih, že delamo na rešitev.</span><span class="sxs-lookup"><span data-stu-id="c6b26-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c6b26-118">Prosimo, da nam vsaj 24 ur za dokončanje rešitev.</span><span class="sxs-lookup"><span data-stu-id="c6b26-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="c6b26-119">Če morate ustvariti novo mesto ekipe, ki ne vključuje skupino Office 365</span><span class="sxs-lookup"><span data-stu-id="c6b26-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


