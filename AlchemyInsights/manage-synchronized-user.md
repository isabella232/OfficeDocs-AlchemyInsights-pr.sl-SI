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
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777693"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Primarnega e-poštnega naslova, spreminjanje uporabniških atributov ali odstranjevanje/brisanje sinhroniziranega uporabnika ni mogoče nastaviti

Če je sinhronizacija imenika omogočena za vaše okolje, ne morete spremeniti nekaterih atributov uporabnika ali predmeta s skrbniškim središčem za Microsoft 365.

Če želite v celoti upravljati sinhronizirane uporabnike in vse njihove atribute, uporabite svoje lokalne uporabnike imenika Active Directory in konzolo za upravljanje skupin (Adsiedit. msc).  

Druga možnost je, da lahko spremenite posamezne uporabnike ali atribute za sinhronizirane uporabnike z uporabo lupine PowerShell, kot je prikazano v teh pogostih primerih: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
