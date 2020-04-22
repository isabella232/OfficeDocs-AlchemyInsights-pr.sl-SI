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
# <a name="upn-sync-disabled"></a>UPN sinhronizacija onemogočena

Če ste začeli sinhronizacijo s storitvijo Azure AD pred 30. marca 2016, zaženite ta ukaz» cmdlet «Azure AD PowerShell, da omogočite samo UPN mehko ujemanje samo za vašo organizacijo:
  
 **Set-MsolDirSyncFeature-funkcija EnableSoftMatchOnUpn-omogoči $True**
  
UPN mehek vžigalica je automatically obrnjen naprej zakaj društvo to starter omedlevičen v Azure AD naprej ali čez marec 30, 2016.
  
Če želite izvedeti več o omogočanju mehkega ujemanja na UPN in drugih funkcijah sinhronizacije, si oglejte [funkcije storitev sinhronizacije storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

