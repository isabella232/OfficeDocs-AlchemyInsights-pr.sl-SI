---
title: Set ClientAccessServerEnabled to True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320372"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Set ClientAccessServerEnabled to True

Če ne morete odpreti šifriranega e-poštnega sporočila in namesto tega vidite prilogo **rpmsg,** izvedite te korake:

1. Povezovalnik, da Exchange Online PowerShell.

    **Opomba:** Če se želite povezati Exchange Online z lupino PowerShell, se morate vpisati z globalnim skrbnikom ali računom Exchange skrbnika.

   a. Odprite Windows PowerShell, nato pa zaženite ta ukaz:`$UserCredential = Get-Credential`
   b. V **Windows PowerShell oknu Zahteva za poverilnice** vnesite službeni ali šolski račun in geslo, c. Kliknite **V redu**. 

2. Zaženite ta ukaz, če želite ustvariti novo sejo:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Zaženite ta ukaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Ukaz `Get-IRMConfiguration` »Zaženi«.

4. Preverite nastavitev **ClientAccessServerEnabled.** 

    a. Če **je nastavitev ClientAccessServerEnabled** nastavljena na **False,** zaženite ta ukaz »cmdlet«: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Namig:** Sejo lupine Powershell vedno zaprite s tem ukazom: `Remove-PSSession $Session`

Če želite več informacij, [glejte Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

