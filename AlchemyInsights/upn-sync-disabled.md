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
# <a name="upn-sync-disabled"></a>Sinhronizacija UPN je onemogočena

Če ste začeli sinhronizacijo s storitvijo Azure AD pred marcem 30, 2016, zaženite ta ukaz» cmdlet «Azure AD PowerShell, da omogočite le mehko ujemanje UPN za vašo organizacijo:
  
 **Set-MsolDirSyncFeature – funkcija EnableSoftMatchOnUpn – omogoči $True**
  
Funkcija UPN Soft Match je samodejno vklopljena za organizacije, ki so se začele sinhronizirati s storitvijo Azure AD na ali po marcu 30, 2016.
  
Če želite izvedeti več o omogočanju mehkega ujemanja v funkciji UPN in drugih funkcijah sinhronizacije, glejte [funkcije sinhronizacije storitve AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

