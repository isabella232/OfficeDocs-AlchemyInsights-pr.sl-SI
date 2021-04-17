---
title: Upravljanje sinhroniziranega uporabnika
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823983"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ni mogoče nastaviti primarnega e-poštnega naslova, spremeniti atribute uporabnika ali odstraniti/izbrisati sinhroniziranega uporabnika

Če je za vaše okolje omogočena sinhronizacija imenika, nekaterih atributov uporabnika ali predmeta ni mogoče spremeniti v skrbniškem središču za Microsoft 365.

Če želite v celoti upravljati sinhronizirane uporabnike in vse njihove atribute, uporabite lokalne uporabnike imenika Active Directory in konzolo za upravljanje skupin (adsiedit.msc).  

Lahko pa spremenite posamezne uporabnike ali atribute za sinhronizirane uporabnike z uporabo lupine PowerShell, kot je prikazano v teh pogostih primerih:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
