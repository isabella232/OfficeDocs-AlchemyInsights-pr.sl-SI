---
title: Teţave pri povezavi SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840567"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="4088c-102">Teţave pri povezavi SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="4088c-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="4088c-103">Če program SharePoint Designer je težave povezave na SharePointovih mestih, poskusite naslednje skupne rešitve.</span><span class="sxs-lookup"><span data-stu-id="4088c-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="4088c-104">1. korak: Preverite, da SharePoint Designer 2013 posodobljen s [servisnim paketom SP1 za SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) in [2 avgust 2016 posodobite SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="4088c-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="4088c-105">2. korak: Jasno lokalnega predpomnilnika datotek:</span><span class="sxs-lookup"><span data-stu-id="4088c-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="4088c-106">Zaprite SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="4088c-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="4088c-107">V lokalnem računalniku, odstranite vse datoteke, ki so v vsakem od teh map.</span><span class="sxs-lookup"><span data-stu-id="4088c-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="4088c-108">%AppData%\Microsoft\Web strežnik Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="4088c-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="4088c-109">%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="4088c-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="4088c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="4088c-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="4088c-111">Odprite SharePoint Designer 2013 in vnesite konto spet, da vidim, če deluje.</span><span class="sxs-lookup"><span data-stu-id="4088c-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="4088c-112">Korak 3: [omogočajo sodobne preverjanje pristnosti za Office 2013 naprej okno načrt](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4088c-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="4088c-113">Korak 4: Administratorji morali **Omogočajo skript po meri** v postavljanje SharePoint Admin Center omogočiti povezavo programa SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="4088c-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="4088c-114">Glej [Dovoli ali prepreči skript po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="4088c-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


