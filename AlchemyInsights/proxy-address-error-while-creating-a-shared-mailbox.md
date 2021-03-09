---
title: Napaka naslova strežnika proxy med ustvarjanjem nabiralnika v skupni rabi
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
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568306"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Napaka naslova strežnika proxy med ustvarjanjem nabiralnika ali drugega predmeta z omogočenimi e-poštnimi sporočili

Če ste poskusili ustvariti predmet z omogočeno e-pošto (nabiralnik, nabiralnik v skupni rabi itd.) in prejeli napako» naslov strežnika proxy» SMTP:alias@domain.com «je že uporabljen... «, je e-poštni naslov, ki ste ga izbrali, že sprejel drug predmet, ki je omogočen za e-pošto v vaši organizaciji.
  
Če želite poiskati uporabnika, skupino, nabiralnik v skupni rabi ali javno mapo, v kateri je ta e-poštni naslov in ga izbrisati ali spremeniti njegov e-poštni naslov. Nato lahko ustvarite nov predmet z omogočenimi e-poštnimi sporočili, ki je na voljo v sproščenem e-poštnem naslovu. Uporabite iskanje na domači strani, da jo poiščete. Uporabite lahko tudi ta ukaz PowerShell za Exchange Online, da ga poiščete:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Če ne želite izbrisati obstoječega e-poštnega naslova, izberite nov e-poštni naslov novega predmeta, ki ga ustvarjate.
  