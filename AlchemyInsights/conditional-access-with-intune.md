---
title: Pogojni dostop z Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28312051"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="351ba-102">Pogojni dostop z Intune</span><span class="sxs-lookup"><span data-stu-id="351ba-102">Conditional Access with Intune</span></span>

<span data-ttu-id="351ba-103">Uporaba **Pogojnega dostopa** z Intune zahteva 3 korakih:</span><span class="sxs-lookup"><span data-stu-id="351ba-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="351ba-p101">Ustvarjanje **Pravilnika za pogojni dostop** , ki opredeljuje, kakšna sredstva so zaščitene, in kaj pogoji morajo biti izpolnjeni za dostop do teh virov. Na primer, naprava mora biti skladna pred dostopom do podjetja email.</span><span class="sxs-lookup"><span data-stu-id="351ba-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="351ba-p102">Ustvarite **Skladnost politike** , da določite nastavitve, ki morajo biti izpolnjeni, preden napravo se šteje ustrežljiv. Na primer, a naprava mora imeti pin vsaj 6 številk, preden se zagovarja skladne.</span><span class="sxs-lookup"><span data-stu-id="351ba-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="351ba-p103">Zagotavljanje **Skladnosti politik** in **Pogojni dostop pravila** so usmerjene v želeno skupino uporabnikov. To lahko zahteva oblikovanje posebnih skupin uporabnikov v Azure storitve Active Directory.</span><span class="sxs-lookup"><span data-stu-id="351ba-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="351ba-110">Preberite več:</span><span class="sxs-lookup"><span data-stu-id="351ba-110">Read more:</span></span>
  
- [<span data-ttu-id="351ba-111">Pogojni dostop do najboljših praks</span><span class="sxs-lookup"><span data-stu-id="351ba-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="351ba-112">Uvod v pogojni dostop</span><span class="sxs-lookup"><span data-stu-id="351ba-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

