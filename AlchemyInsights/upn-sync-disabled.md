---
title: UPN sync invalidi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423580"
---
# <a name="upn-sync-disabled"></a>UPN sync invalidi

Če ste začeli omedlevičen v sinje AD pred 30 marec 2016, zaženite naslednje Azure AD PowerShell cmdlet omogočiti UPN mehko tekmo v organizaciji le:
  
 **Set-MsolDirSyncFeature-značilnost EnableSoftMatchOnUpn-omogoči $True**
  
UPN mehko tekmo je samodejno vklopljeno za organizacije, ki se je začel sinhronizacijo Azure oglas na ali po 30 marec 2016.
  
Če želite izvedeti več o omogočanju mehko tekmo na UPN in drugih omedlevičen zunanja oblika, si oglejte [Azure AD povezavo sinhronizacijsko storitev funkcije](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

