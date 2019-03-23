---
title: Delitev z zunanjim uporabnikom ne deluje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753442"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="8af33-102">Odpravite težave, delitev SharePointovo vsebino z zunanjim uporabnikom</span><span class="sxs-lookup"><span data-stu-id="8af33-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="8af33-103">Poskrbite, zunanja delitev vklopljena v organizaciji:</span><span class="sxs-lookup"><span data-stu-id="8af33-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="8af33-104">Pojdi na [storitev &amp; dodatki stran v Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), in kliknite **mesta**.</span><span class="sxs-lookup"><span data-stu-id="8af33-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="8af33-105">Poskrbite, da nastavitev je obrnil k "O."</span><span class="sxs-lookup"><span data-stu-id="8af33-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="8af33-106">Če je izbrana "Le obstoječe zunanje uporabnike", poskrbite, da zunanjo uporabnik iz Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="8af33-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="8af33-107">Poskrbite, zunanja delitev vklopljen za mesto.</span><span class="sxs-lookup"><span data-stu-id="8af33-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="8af33-108">Klasična mest:</span><span class="sxs-lookup"><span data-stu-id="8af33-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="8af33-109">V klasičnih SharePoint admin center, v levem podoknu kliknite **zbirke mest**.</span><span class="sxs-lookup"><span data-stu-id="8af33-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="8af33-110">Izberite kraj ali kraje, in na traku kliknite **Skupna raba**.</span><span class="sxs-lookup"><span data-stu-id="8af33-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="8af33-111">Mesto ekipa, ki pripada skupini Office 365, ali mesto komunikacije:</span><span class="sxs-lookup"><span data-stu-id="8af33-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="8af33-112">Te nove vrste mesta imajo isto nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če celotno organizacijo nastavitev omogoča izmenjavo datotek prek povezave, ki ne zahtevajo vpis.</span><span class="sxs-lookup"><span data-stu-id="8af33-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="8af33-113">V tem primeru mesta omogočajo izmenjavo z novim in obstoječim zunanjim uporabnikom, ki vpisati.</span><span class="sxs-lookup"><span data-stu-id="8af33-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="8af33-114">Spremeniti nastavitev za določene strani, uporabite novo SharePoint admin center (predogled) ali PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8af33-114">To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell.</span></span> <span data-ttu-id="8af33-115">[Več](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="8af33-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="8af33-116">Nastavitev za zunanji skupno rabo za vse strani lahko bolj omejujoča kot nastavitev celotno organizacijo, vendar ne manj zahtevnimi kot nastavitev za celotno organizacijo.</span><span class="sxs-lookup"><span data-stu-id="8af33-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

