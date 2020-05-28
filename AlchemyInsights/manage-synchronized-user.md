---
title: Upravljanje sinhroniziranega uporabnika
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407366"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Primarnega e-poštnega naslova ni mogoče nastaviti, spremeniti uporabniških atributov ali odstraniti/izbrisati sinhroniziranega uporabnika

Če je sinhronizacija imenika omogočena za vaše okolje, nekaterih atributov uporabnika ali predmeta ni mogoče spremeniti s skrbniškim središčem Microsoft 365.

Če želite v celoti upravljati sinhronizirane uporabnike in vse njihove atribute, uporabite lokalne uporabnike imenika Active Directory in konzolo za upravljanje skupin (Adsiedit. msc).  

Lahko pa tudi spremenite posamezne uporabnike ali atribute za sinhronizirane uporabnike z lupino, kot je prikazano v teh pogostih primerih: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
