---
title: Omejevanje dostopa v SharePointu ali storitvi OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750680"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="5ddc5-102">Omejevanje dostopa v SharePointu ali storitvi OneDrive</span><span class="sxs-lookup"><span data-stu-id="5ddc5-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="5ddc5-103">Dostop do storitev SharePoint online/OneDrive lahko omejite na več načinov.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="5ddc5-104">Te različne metode omejevanja dostopa so opisane spodaj.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="5ddc5-105">**Omejitev dovoljenja**</span><span class="sxs-lookup"><span data-stu-id="5ddc5-105">**Permission Restriction**</span></span>

<span data-ttu-id="5ddc5-106">V SharePoint online in OneDrive za podjetja omejimo dostop do elementov, kot so mesta, datoteke in mape, tako da dovoljujemo dostop le tistim skupinam/posameznikom, ki bi morali imeti dostop.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="5ddc5-107">Prilagajanje dovoljenj za SharePointov seznam ali knjižnico</span><span class="sxs-lookup"><span data-stu-id="5ddc5-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="5ddc5-108">Prilagajanje dovoljenj za SharePointovo mesto</span><span class="sxs-lookup"><span data-stu-id="5ddc5-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="5ddc5-109">Spreminjanje dovoljenj v podmapi</span><span class="sxs-lookup"><span data-stu-id="5ddc5-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="5ddc5-110">Nadzor dostopa iz neupravljanih naprav</span><span class="sxs-lookup"><span data-stu-id="5ddc5-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="5ddc5-111">Kot SharePointov ali globalni skrbnik v Officeu 365 lahko blokirate ali omejite dostop do vsebine SharePointa in storitve OneDrive iz neupravljanih naprav (tisti, ki niso združeni ali združljivi z AD v InTune).</span><span class="sxs-lookup"><span data-stu-id="5ddc5-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="5ddc5-112">**Omejitev omrežne lokacije**</span><span class="sxs-lookup"><span data-stu-id="5ddc5-112">**Network Location Restriction**</span></span>

<span data-ttu-id="5ddc5-113">Kot skrbnik IT-ja lahko nadzirate dostop do virov SharePoint in OneDrive, ki temeljijo na definiranih omrežnih lokacijah, ki jim zaupate.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="5ddc5-114">To je znano tudi kot pravilnik, ki temelji na lokaciji.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-114">This is also known as location-based policy.</span></span> <span data-ttu-id="5ddc5-115">Če želite več informacij, glejte [nadzor dostopa do podatkov SharePoint online in storitve OneDrive na podlagi omrežnega mesta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="5ddc5-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="5ddc5-116">**Omejitev zaklepanja spletnega mesta**</span><span class="sxs-lookup"><span data-stu-id="5ddc5-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="5ddc5-117">V spletnem mestu SharePoint online lahko zaklenete zbirko mest, tako da nima dostopa nihče.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="5ddc5-118">To je nastavljeno prek lupine PowerShell in [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) z lastnini [set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="5ddc5-119">**Omejevanje uporabnikov z ustvarjanjem spletnih mest ali podmest**</span><span class="sxs-lookup"><span data-stu-id="5ddc5-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="5ddc5-120">Kot globalni skrbnik za SharePoint admin ali Office 365 lahko uporabniki ustvarijo in upravljajo lastna SharePointova mesta, določijo, katere vrste mest lahko ustvarijo, in določite lokacijo mest.</span><span class="sxs-lookup"><span data-stu-id="5ddc5-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="5ddc5-121">Če želite več informacij, glejte [upravljanje ustvarjanja mest v SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="5ddc5-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

