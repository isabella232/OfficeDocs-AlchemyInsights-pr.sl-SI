---
title: UPN sync invalidi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489956"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="8d9f5-102">UPN sync invalidi</span><span class="sxs-lookup"><span data-stu-id="8d9f5-102">UPN sync disabled</span></span>

<span data-ttu-id="8d9f5-103">Če ste začeli omedlevičen v sinje AD pred 30 marec 2016, zaženite naslednje Azure AD PowerShell cmdlet omogočiti UPN mehko tekmo v organizaciji le:</span><span class="sxs-lookup"><span data-stu-id="8d9f5-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="8d9f5-104">**Set-MsolDirSyncFeature-značilnost EnableSoftMatchOnUpn-omogoči $True**</span><span class="sxs-lookup"><span data-stu-id="8d9f5-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="8d9f5-105">UPN mehko tekmo je samodejno vklopljeno za organizacije, ki se je začel sinhronizacijo Azure oglas na ali po 30 marec 2016.</span><span class="sxs-lookup"><span data-stu-id="8d9f5-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="8d9f5-106">Če želite izvedeti več o omogočanju mehko tekmo na UPN in drugih omedlevičen zunanja oblika, si oglejte [Azure AD povezavo sinhronizacijsko storitev funkcije](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="8d9f5-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

