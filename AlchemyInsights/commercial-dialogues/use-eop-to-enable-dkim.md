---
title: Uporaba Exchange Online PowerShell za omogočanje skripta DKIM za določeno domeno
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070332"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Uporaba Exchange Online PowerShell za omogočanje skripta DKIM za določeno domeno

Če ne morete ustvariti zapisov DKIM DNS v skrbniškem središču, poskusite uporabiti Exchange Online PowerShell. 

Če želite ustvariti zapis DNS DKIM s Exchange Online PowerShell, izvedite te korake:

1. Odprite Windows PowerShell kot skrbnik in zaženite te ukaze v opisanem zaporedju:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Če imate težave pri vzpostavljanju povezave z Exchange Online PowerShell, [Povezovalnik za Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Ko imate vzpostavljeno povezavo z Exchange Online PowerShell, zaženite ta ukaz:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Ko je zgornji ukaz uspešno izveden, zaženite ta ukaz, da prekinete sejo Exchange Online PowerShell:

    `Remove-PSSession $Session` 



