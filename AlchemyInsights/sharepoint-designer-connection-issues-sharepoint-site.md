---
title: Težave s povezavo za SharePoint Designer
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511560"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="55ec3-102">Težave s povezavo za SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="55ec3-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="55ec3-103">Če SharePoint Designer doživlja težave s povezavo s SharePointovimi mesti, poskusite z naslednjimi skupnimi rešitvami.</span><span class="sxs-lookup"><span data-stu-id="55ec3-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="55ec3-104">Korak 1: Preverite, ali je SharePoint Designer 2013 posodobljen s [servisnim paketom SharePoint Designer 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) in [avgustom 2, 2016 posodobitev za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="55ec3-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="55ec3-105">2. korak: počistite lokalne datoteke predpomnilnika:</span><span class="sxs-lookup"><span data-stu-id="55ec3-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="55ec3-106">Zaprite SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="55ec3-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="55ec3-107">V lokalnem računalniku odstranite vse datoteke, najdene v vsaki od teh map.</span><span class="sxs-lookup"><span data-stu-id="55ec3-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="55ec3-108">%AppData%\microsoft\spletni strežnik Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="55ec3-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="55ec3-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="55ec3-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="55ec3-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="55ec3-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="55ec3-111">Odprite SharePoint Designer 2013 in znova vnesite račun, da preverite, ali deluje.</span><span class="sxs-lookup"><span data-stu-id="55ec3-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="55ec3-112">Korak 3: [omogočite sodobno preverjanje pristnosti za Office 2013 v napravah s sistemom Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="55ec3-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="55ec3-113">Korak 4: skrbniki bodo morali **dovoliti skript po meri** v nastavitvah SharePoint skrbniško središče, da se omogoči povezava SharePointovega oblikovalca.</span><span class="sxs-lookup"><span data-stu-id="55ec3-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="55ec3-114">Če želite več informacij, glejte [Omogočanje ali preprečevanje skripta po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .</span><span class="sxs-lookup"><span data-stu-id="55ec3-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


