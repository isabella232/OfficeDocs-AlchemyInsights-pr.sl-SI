---
title: Omejevanje dostopa v SharePointu ali OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700471"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="0e3f2-102">Omejevanje dostopa v SharePointu ali OneDrive</span><span class="sxs-lookup"><span data-stu-id="0e3f2-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="0e3f2-103">Dostop do storitev SharePoint online/OneDrive lahko omejite na več načinov.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="0e3f2-104">Te različne metode omejevanja dostopa so opisane spodaj.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="0e3f2-105">**Omejitev dovoljenj**</span><span class="sxs-lookup"><span data-stu-id="0e3f2-105">**Permission Restriction**</span></span>

<span data-ttu-id="0e3f2-106">V storitvi SharePoint online in OneDrive za podjetja omejimo dostop do elementov, kot so mesta, datoteke in mape, in sicer tako, da dodeli le dostop do tistih skupin/posameznikov, ki bi morali imeti dostop.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="0e3f2-107">Prilagajanje dovoljenj za SharePointov seznam ali knjižnico</span><span class="sxs-lookup"><span data-stu-id="0e3f2-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="0e3f2-108">Prilagajanje dovoljenj za SharePointovo mesto</span><span class="sxs-lookup"><span data-stu-id="0e3f2-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="0e3f2-109">Spreminjanje dovoljenj v podmapi</span><span class="sxs-lookup"><span data-stu-id="0e3f2-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="0e3f2-110">Nadzor dostopa v neupravljanih napravah</span><span class="sxs-lookup"><span data-stu-id="0e3f2-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="0e3f2-111">Kot SharePoint ali globalni skrbnik lahko blokirate ali omejite dostop do SharePointovih in OneDrive vsebine iz neupravljanih naprav (tistih, ki niso povezani s hibridnim OGLASom ali pa so združljivi z InTune).</span><span class="sxs-lookup"><span data-stu-id="0e3f2-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="0e3f2-112">**Omejitev omrežnega mesta**</span><span class="sxs-lookup"><span data-stu-id="0e3f2-112">**Network Location Restriction**</span></span>

<span data-ttu-id="0e3f2-113">Kot skrbnik za IT lahko nadzorujete dostop do SharePointovih in OneDrive virov na podlagi določenih omrežnih mest, ki jim zaupate.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="0e3f2-114">To je znana tudi kot pravilnik, ki temelji na lokaciji.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-114">This is also known as location-based policy.</span></span> <span data-ttu-id="0e3f2-115">Če želite več informacij, glejte [nadzor dostopa do podatkov v storitvi SharePoint online in OneDrive, ki temeljijo na omrežnem mestu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="0e3f2-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="0e3f2-116">**Omejitev zaklepanja mesta**</span><span class="sxs-lookup"><span data-stu-id="0e3f2-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="0e3f2-117">V storitvi SharePoint online lahko zaklenete zbirko mest, tako da nihče nima dostopa.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="0e3f2-118">To je nastavljeno prek lupine PowerShell in storitve [SharePoint online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) z lastnostjo [set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="0e3f2-119">**Omejevanje uporabnikov pred ustvarjanjem mest ali podmest**</span><span class="sxs-lookup"><span data-stu-id="0e3f2-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="0e3f2-120">Kot skrbnik za SharePoint ali globalni skrbnik lahko uporabnikom omogočite, da ustvarijo in upravljajo svoja SharePointova mesta, določajo, katere vrste mest, ki jih lahko ustvarijo, in določijo mesto mesta.</span><span class="sxs-lookup"><span data-stu-id="0e3f2-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="0e3f2-121">Če želite več informacij, glejte [upravljanje ustvarjanja mesta v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="0e3f2-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

