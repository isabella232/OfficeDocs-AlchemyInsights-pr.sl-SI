---
title: Pogojni dostop z InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505010"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="8f08b-102">Pogojni dostop z InTune</span><span class="sxs-lookup"><span data-stu-id="8f08b-102">Conditional Access with Intune</span></span>

<span data-ttu-id="8f08b-103">Uporaba **pogojnega dostopa** z InTune zahteva 3 korake:</span><span class="sxs-lookup"><span data-stu-id="8f08b-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="8f08b-104">Ustvarite **pravilnik pogojnega dostopa** , ki določa, kateri viri so zaščiteni, in katere pogoje je treba izpolniti za dostop do teh virov.</span><span class="sxs-lookup"><span data-stu-id="8f08b-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="8f08b-105">Naprava mora biti na primer skladna pred dostopom do e-pošte podjetja.</span><span class="sxs-lookup"><span data-stu-id="8f08b-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="8f08b-106">Ustvarite **pravilnik o skladnosti** , če želite določiti nastavitve, ki morajo biti izpolnjene, preden se naprava šteje za združljivo.</span><span class="sxs-lookup"><span data-stu-id="8f08b-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="8f08b-107">Naprava mora imeti na primer PIN vsaj 6 števk, preden se šteje za skladno.</span><span class="sxs-lookup"><span data-stu-id="8f08b-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="8f08b-108">Zagotavljanje, da **Pravilniki o skladnosti** in pravilniki o **pogojnem dostopu** ciljajo na želene skupine uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="8f08b-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="8f08b-109">To lahko zahteva ustvarjanje določenih skupin uporabnikov v storitvi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8f08b-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="8f08b-110">Preberite več:</span><span class="sxs-lookup"><span data-stu-id="8f08b-110">Read more:</span></span>
  
- [<span data-ttu-id="8f08b-111">Najboljši postopki za pogojni dostop</span><span class="sxs-lookup"><span data-stu-id="8f08b-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="8f08b-112">Uvod v pogojni dostop</span><span class="sxs-lookup"><span data-stu-id="8f08b-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

