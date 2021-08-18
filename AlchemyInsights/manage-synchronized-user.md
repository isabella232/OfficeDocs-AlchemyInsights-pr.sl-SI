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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114794"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Ni mogoče nastaviti primarnega e-poštnega naslova, spremeniti atribute uporabnika ali odstraniti/izbrisati sinhroniziranega uporabnika

Če je za vaše okolje omogočena sinhronizacija imenika, nekaterih atributov uporabnika ali predmeta ni mogoče spremeniti z Skrbniško središče za Microsoft 365.

Če želite v celoti upravljati sinhronizirane uporabnike in vse njihove atribute, uporabite lokalne uporabnike imenika Active Directory in konzolo za upravljanje skupin (adsiedit.msc).  

Lahko pa spremenite posamezne uporabnike ali atribute za sinhronizirane uporabnike z uporabo lupine PowerShell, kot je prikazano v teh pogostih primerih:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
