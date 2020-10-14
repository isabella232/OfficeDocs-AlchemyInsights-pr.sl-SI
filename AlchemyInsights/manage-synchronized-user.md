---
title: Upravljanje sinhroniziranega uporabnika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451416"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Primarnega e-poštnega naslova, spreminjanje uporabniških atributov ali odstranjevanje/brisanje sinhroniziranega uporabnika ni mogoče nastaviti

Če je sinhronizacija imenika omogočena za vaše okolje, ne morete spremeniti nekaterih atributov uporabnika ali predmeta s skrbniškim središčem za Microsoft 365.

Če želite v celoti upravljati sinhronizirane uporabnike in vse njihove atribute, uporabite svoje lokalne uporabnike imenika Active Directory in konzolo za upravljanje skupin (Adsiedit. msc).  

Druga možnost je, da lahko spremenite posamezne uporabnike ali atribute za sinhronizirane uporabnike z uporabo lupine PowerShell, kot je prikazano v teh pogostih primerih:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
