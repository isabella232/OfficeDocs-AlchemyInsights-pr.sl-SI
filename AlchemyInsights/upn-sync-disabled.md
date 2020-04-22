---
title: UPN sinhronizacija onemogočena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726120"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="0416d-102">UPN sinhronizacija onemogočena</span><span class="sxs-lookup"><span data-stu-id="0416d-102">UPN sync disabled</span></span>

<span data-ttu-id="0416d-103">Če ste začeli sinhronizacijo s storitvijo Azure AD pred 30. marca 2016, zaženite ta ukaz» cmdlet «Azure AD PowerShell, da omogočite samo UPN mehko ujemanje samo za vašo organizacijo:</span><span class="sxs-lookup"><span data-stu-id="0416d-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="0416d-104">**Set-MsolDirSyncFeature-funkcija EnableSoftMatchOnUpn-omogoči $True**</span><span class="sxs-lookup"><span data-stu-id="0416d-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="0416d-105">UPN mehek vžigalica je automatically obrnjen naprej zakaj društvo to starter omedlevičen v Azure AD naprej ali čez marec 30, 2016.</span><span class="sxs-lookup"><span data-stu-id="0416d-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="0416d-106">Če želite izvedeti več o omogočanju mehkega ujemanja na UPN in drugih funkcijah sinhronizacije, si oglejte [funkcije storitev sinhronizacije storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="0416d-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

