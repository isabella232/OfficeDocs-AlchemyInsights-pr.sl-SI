---
title: Uporaba storitve PowerShell za Exchange Online za omogočanje DKIM za določeno domeno
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525244"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Uporaba storitve PowerShell za Exchange Online za omogočanje DKIM za določeno domeno

Če v skrbniškem središču ne morete ustvariti DKIM zapisov DNS, poskusite uporabiti PowerShell za Exchange Online. 

Če želite ustvariti zapis DNS DKIM s storitvijo Exchange Online PowerShell, izvedite te korake:

1. Odprite Windows PowerShell kot skrbnik in v opisanem zaporedju zaženite te ukaze:

    v. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Če imate težave z vzpostavljanjem povezave s storitvijo Exchange Online PowerShell, glejte [Vzpostavljanje povezave s storitvijo Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Ko imate vzpostavljeno povezavo s storitvijo Exchange Online PowerShell, zaženite ta ukaz:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Ko je zgornji ukaz uspešno izveden, zaženite ta ukaz, da prekinete sejo PowerShell za Exchange Online:

    `Remove-PSSession $Session` 



