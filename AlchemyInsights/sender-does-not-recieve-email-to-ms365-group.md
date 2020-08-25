---
title: Pošiljatelj ne prejme e-pošte, poslane v skupino Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872178"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Pošiljatelj ne prejme e-pošte, poslane v skupino Microsoft 365

Pošiljatelj e-poštnega sporočila v skupino Microsoft 365 privzeto ne prejme kopije sporočila v mapi» Prejeto «, tudi če je pošiljatelj član skupine.

S tem ukazom» EKSO PowerShell «lahko pošiljatelju dovolite, da prejme kopijo posamezne e-pošte, ki jo pošljejo v skupino Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Če želite omogočiti nastavitev za vse nabiralnike hkrati:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Opomba** Spremembe te nastavitve trajajo do ene ure.