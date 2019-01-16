---
title: Delitev z zunanjim uporabnikom ne deluje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 305b3891e6c83e27b5c55c13757640e6e9d51a81
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28312744"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="34d0b-102">Odpravite težave, delitev SharePointovo vsebino z zunanjim uporabnikom</span><span class="sxs-lookup"><span data-stu-id="34d0b-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="34d0b-103">Poskrbite, zunanja delitev vklopljena v organizaciji:</span><span class="sxs-lookup"><span data-stu-id="34d0b-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="34d0b-104">Pojdi na [storitev &amp; dodatki stran v skrbniškem središču za Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), in kliknite **mesta**.</span><span class="sxs-lookup"><span data-stu-id="34d0b-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="34d0b-p101">Poskrbite, da nastavitev je obrnil k "O." Če je izbrana "Le obstoječe zunanje uporabnike", se prepričajte, zunanjo uporabnik je prisluškovati v skrbniškem središču za Office 365.</span><span class="sxs-lookup"><span data-stu-id="34d0b-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="34d0b-p102">Poskrbite, zunanja delitev vklopljen za mesto. Klasična mest:</span><span class="sxs-lookup"><span data-stu-id="34d0b-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="34d0b-109">V klasičnih SharePoint admin center, v levem podoknu kliknite **zbirke mest**.</span><span class="sxs-lookup"><span data-stu-id="34d0b-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="34d0b-110">Izberite kraj ali kraje, in na traku kliknite **Skupna raba**.</span><span class="sxs-lookup"><span data-stu-id="34d0b-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="34d0b-111">Mesto ekipa, ki pripada skupini Office 365, ali mesto komunikacije:</span><span class="sxs-lookup"><span data-stu-id="34d0b-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="34d0b-p103">Te nove vrste mesta imajo isto nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če celotno organizacijo nastavitev omogoča izmenjavo datotek prek povezave, ki ne zahtevajo vpis. V tem primeru mesta omogočajo izmenjavo z novim in obstoječim zunanjim uporabnikom, ki vpisati. Spremeniti nastavitev za določene strani, uporabite novo SharePoint admin center (predogled) ali PowerShell. [Več](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="34d0b-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="34d0b-116">Nastavitev za zunanji skupno rabo za vse strani lahko bolj omejujoča kot nastavitev celotno organizacijo, vendar ne manj zahtevnimi kot nastavitev za celotno organizacijo.</span><span class="sxs-lookup"><span data-stu-id="34d0b-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

