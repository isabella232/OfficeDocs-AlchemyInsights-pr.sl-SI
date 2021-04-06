---
title: Obnovitev izbrisane skupine v storitvi Microsoft 365
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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597459"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Obnovitev izbrisane skupine v storitvi Microsoft 365

Izbrisano skupino v storitvi Microsoft 365 ali Microsoft Teams lahko obnovite v 30 dneh od izbrisa.

1. Pojdite v [Skrbniško središče za Microsoft 365](https://aka.ms/RestoreDeletedGroup) in se prijavite ter navedite izbrisane skupine in skupine.

    **Opomba:** Prijavite se z računom, ki je dodeljen skrbniku najemnika ali skrbniški vlogi skupine.

1. Izberite izbrisano skupino/skupino Storitve Microsoft 365/Teams, ki jo želite obnoviti, in **kliknite obnovi skupino.**

    Če skupine ni mogoče obnoviti zaradi naslova SMTP v sporu, uporabite ta ukaz, da najdete predmet, ki povzroča spor, in odstranite naslov SMTP:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Opomba:** V nekaterih primerih lahko traja do 24 ur, da so skupina in vsi njeni podatki obnovljeni.

    Če želite več informacij ali če želite izvedeti, kako obnovite skupine s storitvijo PowerShell, glejte Obnovitev izbrisane skupine v storitvi [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)