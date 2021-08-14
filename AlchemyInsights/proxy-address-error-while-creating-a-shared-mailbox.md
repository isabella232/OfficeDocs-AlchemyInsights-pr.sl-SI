---
title: Napaka naslova proxy med ustvarjanjem nabiralnika v skupni rabi
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062924"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Napaka naslova proxy med ustvarjanjem nabiralnika ali drugega predmeta z omogočeno e-pošto

Če ste poskusili ustvariti predmet z omogočeno e-pošto (nabiralnik, nabiralnik v skupni rabi itd.) in prejeli napako »Naslov proxy »SMTP:alias@domain.com« je že v uporabi ...«, izbrani e-poštni naslov že uporablja drug predmet, ki omogoča e-pošto v vaši organizaciji.
  
Poiskati morate uporabnika, skupino, nabiralnik v skupni rabi ali javno mapo s tem e-poštnim naslovom in ga izbrisati ali spremeniti njegov e-poštni naslov. Nato lahko ustvarite nov predmet, ki omogoča e-pošto, s prostim e-poštnim naslovom. Poiščite ga s funkcijo »Iskanje« na domači strani. Uporabite lahko tudi ta ukaz Exchange Online PowerShell, da ga poiščete:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Če ne želite izbrisati obstoječega e-poštnega naslova, izberite nov e-poštni naslov za novi predmet, ki ga ustvarjate.
  