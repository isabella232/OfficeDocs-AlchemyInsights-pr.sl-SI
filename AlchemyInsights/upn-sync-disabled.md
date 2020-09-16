---
title: Sinhronizacija UPN je onemogočena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749530"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="6e5ef-102">Sinhronizacija UPN je onemogočena</span><span class="sxs-lookup"><span data-stu-id="6e5ef-102">UPN sync disabled</span></span>

<span data-ttu-id="6e5ef-103">Če ste začeli sinhronizacijo s storitvijo Azure AD pred marcem 30, 2016, zaženite ta ukaz» cmdlet «Azure AD PowerShell, da omogočite le mehko ujemanje UPN za vašo organizacijo:</span><span class="sxs-lookup"><span data-stu-id="6e5ef-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="6e5ef-104">**Set-MsolDirSyncFeature – funkcija EnableSoftMatchOnUpn – omogoči $True**</span><span class="sxs-lookup"><span data-stu-id="6e5ef-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="6e5ef-105">Funkcija UPN Soft Match je samodejno vklopljena za organizacije, ki so se začele sinhronizirati s storitvijo Azure AD na ali po marcu 30, 2016.</span><span class="sxs-lookup"><span data-stu-id="6e5ef-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="6e5ef-106">Če želite izvedeti več o omogočanju mehkega ujemanja v funkciji UPN in drugih funkcijah sinhronizacije, glejte [funkcije sinhronizacije storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="6e5ef-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

