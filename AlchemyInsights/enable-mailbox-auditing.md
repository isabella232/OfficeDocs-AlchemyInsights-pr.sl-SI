---
title: Omogočanje nadzora nabiralnika
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
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806307"
---
# <a name="enable-mailbox-auditing"></a>Omogočanje nadzora nabiralnika

Če želite omogočiti nadzor nabiralnika za enega uporabnika ali celotno organizacijo, morajo biti te ukaze» cmdlet «zagnane iz oddaljenega dodatka Power Shell:
  
 **En uporabnik**
  
Nastavitev nabiralnika – identiteta» Jane Dow «– AuditEnabled $true
  
 **Organizaciji**
  
Get-Mailbox-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Nastavitev nabiralnika – AuditEnabled $true
  
[več](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

