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
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502247"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="03c1a-102">Odpravite težave, delitev SharePointovo vsebino z zunanjim uporabnikom</span><span class="sxs-lookup"><span data-stu-id="03c1a-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="03c1a-103">Poskrbite, zunanja delitev vklopljena v organizaciji:</span><span class="sxs-lookup"><span data-stu-id="03c1a-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="03c1a-104">Pojdi na [storitev &amp; dodatki stran v Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), in kliknite **mesta**.</span><span class="sxs-lookup"><span data-stu-id="03c1a-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="03c1a-105">Poskrbite, da nastavitev je obrnil k "O."</span><span class="sxs-lookup"><span data-stu-id="03c1a-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="03c1a-106">Če je izbrana "Le obstoječe zunanje uporabnike", poskrbite, da zunanjo uporabnik iz Microsoft 365 admin center.</span><span class="sxs-lookup"><span data-stu-id="03c1a-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="03c1a-107">Poskrbite, zunanja delitev vklopljen za mesto.</span><span class="sxs-lookup"><span data-stu-id="03c1a-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="03c1a-108">Klasična mest:</span><span class="sxs-lookup"><span data-stu-id="03c1a-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="03c1a-109">V novi SharePoint admin center, v levem podoknu kliknite **mesta**.</span><span class="sxs-lookup"><span data-stu-id="03c1a-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="03c1a-110">Izberite kraj ali kraje, in na traku kliknite **Skupna raba**.</span><span class="sxs-lookup"><span data-stu-id="03c1a-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="03c1a-111">Mesto ekipa, ki pripada skupini Office 365, ali mesto komunikacije:</span><span class="sxs-lookup"><span data-stu-id="03c1a-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="03c1a-112">Te nove vrste mesta imajo isto nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če celotno organizacijo nastavitev omogoča izmenjavo datotek prek povezave, ki ne zahtevajo vpis.</span><span class="sxs-lookup"><span data-stu-id="03c1a-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="03c1a-113">V tem primeru mesta omogočajo izmenjavo z novim in obstoječim zunanjim uporabnikom, ki vpisati.</span><span class="sxs-lookup"><span data-stu-id="03c1a-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="03c1a-114">Spremeniti nastavitev za določene strani, uporabite novo SharePoint admin center ali PowerShell.</span><span class="sxs-lookup"><span data-stu-id="03c1a-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="03c1a-115">[Več](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="03c1a-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="03c1a-116">Nastavitev za zunanji skupno rabo za vse strani lahko bolj omejujoča kot nastavitev celotno organizacijo, vendar ne manj zahtevnimi kot nastavitev za celotno organizacijo.</span><span class="sxs-lookup"><span data-stu-id="03c1a-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

