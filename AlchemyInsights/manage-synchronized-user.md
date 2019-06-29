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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380521"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Ni mogoče nastaviti primarni e-poštni naslov ali spremenite atribute

Če je omogočena sinhronizacija imenika za vaš okolja ni mogoče spremeniti nekaterih atributov uporabnika ali predmet, z uporabo Admin Center.
Da v celoti upravljati sinhronizirani uporabniki in njihove lastnosti, uporabite vaš lokalni imenik active directory uporabniki in skupine konzolo za upravljanje (adsiedit.msc).  

Alternativno, lahko spremenite posamezne uporabnike ali atributi za sinhronizirani uporabniki z uporabo powershell, kot je prikazano v teh pogosti primeri: 
- Set-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Testni uporabnik" - priimek "Uporabnik"-naslov "Manager"-oddelek "HR"
- Odstrani-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com