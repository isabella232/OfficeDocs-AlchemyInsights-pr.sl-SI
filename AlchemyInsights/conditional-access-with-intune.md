---
title: Pogojni dostop z Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505010"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="d7791-102">Pogojni dostop z Intune</span><span class="sxs-lookup"><span data-stu-id="d7791-102">Conditional Access with Intune</span></span>

<span data-ttu-id="d7791-103">Uporaba **Pogojnega dostopa** z Intune zahteva 3 korakih:</span><span class="sxs-lookup"><span data-stu-id="d7791-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="d7791-104">Ustvarjanje **Pravilnika za pogojni dostop** , ki opredeljuje, kakšna sredstva so zaščitene, in kaj pogoji morajo biti izpolnjeni za dostop do teh virov.</span><span class="sxs-lookup"><span data-stu-id="d7791-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="d7791-105">Na primer, naprava mora biti skladna pred dostopom do podjetja email.</span><span class="sxs-lookup"><span data-stu-id="d7791-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="d7791-106">Ustvarite **Skladnost politike** , da določite nastavitve, ki morajo biti izpolnjeni, preden napravo se šteje ustrežljiv.</span><span class="sxs-lookup"><span data-stu-id="d7791-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="d7791-107">Na primer, a naprava mora imeti pin vsaj 6 številk, preden se zagovarja skladne.</span><span class="sxs-lookup"><span data-stu-id="d7791-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="d7791-108">Zagotavljanje **Skladnosti politik** in **Pogojni dostop pravila** so usmerjene v želeno skupino uporabnikov.</span><span class="sxs-lookup"><span data-stu-id="d7791-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="d7791-109">To lahko zahteva oblikovanje posebnih skupin uporabnikov v Azure storitve Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d7791-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="d7791-110">Preberite več:</span><span class="sxs-lookup"><span data-stu-id="d7791-110">Read more:</span></span>
  
- [<span data-ttu-id="d7791-111">Pogojni dostop do najboljših praks</span><span class="sxs-lookup"><span data-stu-id="d7791-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="d7791-112">Uvod v pogojni dostop</span><span class="sxs-lookup"><span data-stu-id="d7791-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

