---
title: Nastavitev ClientAccessServerEnabled na True
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749976"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Nastavitev ClientAccessServerEnabled na True

Če ne morete odpreti šifriranega e-poštnega sporočila in namesto tega vidite Prilogo **rpmsg** , izvedite te korake:

1. Vzpostavite povezavo s storitvijo PowerShell Exchange Online.

> [!NOTE]
> Če želite vzpostaviti povezavo s storitvijo PowerShell Exchange Online, se morate vpisati s skrbniškim računom za globalni skrbnik ali Exchange.

   v. Odprite Windows PowerShell in zaženite ta ukaz: `$UserCredential = Get-Credential`
b. V pogovornem oknu **zahteva za poverilnice Windows PowerShell** vnesite službeni ali šolski račun in geslo, c. Kliknite **V redu**. 

2. Če želite ustvariti novo sejo, zaženite ta ukaz:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    v. Zaženite ta ukaz:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Ukaz» Zaženi «.

4. Preverite nastavitev **ClientAccessServerEnabled** . 

    v. Če je nastavitev **ClientAccessServerEnabled** nastavljena na» **FALSE**«, zaženite ta ukaz» cmdlet «: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Vedno zaprite sejo lupine PowerShell s tem ukazom: `Remove-PSSession $Session`

Če želite več informacij, glejte [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

