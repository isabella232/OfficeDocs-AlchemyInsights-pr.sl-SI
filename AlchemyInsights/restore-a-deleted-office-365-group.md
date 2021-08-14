---
title: Obnovitev izbrisane Microsoft 365 skupine
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
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959042"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovitev izbrisane Microsoft 365 skupine

Izbrisano skupino ali skupino Microsoft 365 lahko obnovite Microsoft Teams v 30 dneh od izbrisa.

1. Pojdite v [Skrbniško središče za Microsoft 365,](https://aka.ms/RestoreDeletedGroup) da se prijavite na seznam izbrisanih skupin in skupin.

    **Opomba:** Prijavite se z računom, ki je dodeljen skrbniku najemnika ali skrbniški vlogi skupine.

1. Izberite izbrisano skupino Microsoft 365/skupine Teams ki jo želite obnoviti, in kliknite **obnovi skupino.**

    Če skupine ni mogoče obnoviti zaradi naslova SMTP v sporu, uporabite ta ukaz, da najdete predmet, ki povzroča spor, in odstranite naslov SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Opomba:** V nekaterih primerih lahko traja do 24 ur, da so skupina in vsi njeni podatki obnovljeni.

    Če želite več informacij ali če želite izvedeti, kako obnovite skupine s storitvijo PowerShell, [glejte Obnovitev izbrisane Microsoft 365 skupine.](https://go.microsoft.com/fwlink/?linkid=867802)