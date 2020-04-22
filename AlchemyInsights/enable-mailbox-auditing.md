---
title: Omogočanje revizije nabiralnika
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
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703587"
---
# <a name="enable-mailbox-auditing"></a>Omogočanje revizije nabiralnika

Če želite omogočiti nadzor nabiralnika za enega samega uporabnika ali celotno organizacijo, mora ta ukaz» cmdlet «zagnati iz oddaljene lupine:
  
 **En uporabnik**
  
Set-Mailbox-identiteta "Jane Dow"-AuditEnabled $true
  
 **Organizacija**
  
Get-nabiralnik-ResultSize neomejeno-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true
  
[več](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

