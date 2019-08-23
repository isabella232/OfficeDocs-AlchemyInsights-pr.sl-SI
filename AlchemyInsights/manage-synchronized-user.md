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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542020"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Ni mogoče nastaviti primarni e-poštni naslov ali spremenite atribute

Če sinhronizacija imenika omogočena za vaše okolje, ni mogoče spremeniti nekaterih atributov uporabnika ali predmet, z uporabo Microsoft 365 admin center.

Da v celoti upravljati sinhronizirani uporabniki in njihove lastnosti, uporabite vaš lokalni imenik active directory uporabniki in skupine konzolo za upravljanje (adsiedit.msc).  

Alternativno, lahko spremenite posamezne uporabnike ali atributi za sinhronizirani uporabniki z uporabo powershell, kot je prikazano v teh pogosti primeri: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testni uporabnik" - priimek "Uporabnik"-naslov "Manager"-oddelek "HR"
- Odstrani-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com