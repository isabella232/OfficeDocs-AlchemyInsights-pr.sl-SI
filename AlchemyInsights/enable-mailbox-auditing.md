---
title: Omogočite nabiralnika nadzor
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500298"
---
# <a name="enable-mailbox-auditing"></a>Omogočite nabiralnika nadzor

Da omogočite nabiralnika nadzor za enega uporabnika ali celotno organizacijo iz oddaljenih PowerShellu zaženite naslednje ukaze »cmdlet« :
  
 **Posamezen uporabnik**
  
Nabor-nabiralnika - Identity "Jane Dow" - AuditEnabled $true
  
 Organization
  
Get-poštni nabiralnik - ResultSize neomejeno - Filter {RecipientTypeDetails - eq "UserMailbox"} | Set-Mailbox - AuditEnabled $true
  
Preberite več o tem.
  

