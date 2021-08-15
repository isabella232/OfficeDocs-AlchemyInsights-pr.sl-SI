---
title: Sinhronizacija UPN je onemogočena
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038128"
---
# <a name="upn-sync-disabled"></a>Sinhronizacija UPN je onemogočena

Če ste začeli sinhronizirati z imenikom Azure AD pred 30. marcem 2016, zaženite ta ukaz »cmdlet« Azure AD PowerShell, da omogočite le mehko ujemanje upn za vašo organizacijo:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Mehek zadetek upn je samodejno vklopljen za organizacije, ki so začele sinhronizirati z imenikom Azure AD 30. marca 2016 ali po tem.
  
Če želite izvedeti več o omogočanju mehkega ujemanja v UPN-jih in drugih funkcijah sinhronizacije, glejte [Funkcije storitve Povezovalnik sinhronizacije imenika Azure AD.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

