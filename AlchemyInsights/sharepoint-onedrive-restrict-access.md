---
title: Omejevanje dostopa v SharePoint ali OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223728"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="335ea-102">Omejevanje dostopa v SharePoint ali OneDrive</span><span class="sxs-lookup"><span data-stu-id="335ea-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="335ea-103">Obstaja veliko načinov za preprečevanje dostopa do storitve SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="335ea-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="335ea-104">Te različne metode za omejitev dostopa so opisani spodaj.</span><span class="sxs-lookup"><span data-stu-id="335ea-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="335ea-105">**Dovoljenje omejitve**</span><span class="sxs-lookup"><span data-stu-id="335ea-105">**Permission Restriction**</span></span>

<span data-ttu-id="335ea-106">V SharePoint Online in OneDrive za poslovanje, smo omejiti dostop do predmetov, kot so spletna mesta, datoteke in mape samo odobri dostop do tistim skupinam/posameznikom, ki bi morali imeti dostop.</span><span class="sxs-lookup"><span data-stu-id="335ea-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="335ea-107">Prilagodite dovoljenj za SharePointov seznam ali knjižnico</span><span class="sxs-lookup"><span data-stu-id="335ea-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="335ea-108">Prilagodite dovoljenja mesta SharePoint</span><span class="sxs-lookup"><span data-stu-id="335ea-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="335ea-109">Spremenite dovoljenja, podmape</span><span class="sxs-lookup"><span data-stu-id="335ea-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="335ea-110">Nadzor dostopa iz neupravljane naprave</span><span class="sxs-lookup"><span data-stu-id="335ea-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="335ea-111">Kot SharePoint ali svetovnih admin v Office 365, lahko blokirate ali omejiti dostop do vsebin, SharePoint in OneDrive iz neupravljane naprave (teh hibridnih AD pridružil ali ustrežljiv v Intune).</span><span class="sxs-lookup"><span data-stu-id="335ea-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="335ea-112">**Omrežno mesto omejitev**</span><span class="sxs-lookup"><span data-stu-id="335ea-112">**Network Location Restriction**</span></span>

<span data-ttu-id="335ea-113">Kot IT admin, lahko nadzor dostopa do virov SharePoint in OneDrive, na osnovi določenih omrežnih mest, ki jim zaupate.</span><span class="sxs-lookup"><span data-stu-id="335ea-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="335ea-114">To je znana tudi kot namestitev-osnova politike.</span><span class="sxs-lookup"><span data-stu-id="335ea-114">This is also known as location-based policy.</span></span> <span data-ttu-id="335ea-115">Če želite več informacij, si oglejte [pregled postranski v SharePoint Online in OneDrive podatke, ki temeljijo na omrežno mesto](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="335ea-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="335ea-116">**Omejitve mesta Lock**</span><span class="sxs-lookup"><span data-stu-id="335ea-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="335ea-117">V SharePoint Online imate sposobnost za zaklepanje določitvi mest, tako da nihče ni dostopa.</span><span class="sxs-lookup"><span data-stu-id="335ea-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="335ea-118">To se nahaja preko PowerShell in [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) uporabite lastnost - LockState [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="335ea-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="335ea-119">**Določim, da ustvarjanje mest ali podmesta**</span><span class="sxs-lookup"><span data-stu-id="335ea-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="335ea-120">Kot SharePoint admin ali Office 365 svetovnih admin, lahko pustite vaš uporabnik ustvariti in upravljati svoje lastne SharePointovih mest, ugotoviti, kakšne strani, ki jih lahko ustvarite, določite lokacijo mesta.</span><span class="sxs-lookup"><span data-stu-id="335ea-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="335ea-121">Če želite več informacij, si oglejte [Ustvarjanje upravljanje mesta v SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="335ea-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

