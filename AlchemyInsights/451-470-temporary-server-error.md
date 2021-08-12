---
title: 451 4.7.0 Začasna napaka strežnika. Poskusite znova pozneje. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812591"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Začasna napaka strežnika. Poskusite znova pozneje. PRX4

Pri pošiljanju e-pošte prek storitve Smarthost »smtp.office365.com« lahko pride do težave z načinom pošiljanja prek odjemalca SMTP in prejmete napako: »Napaka začasnega strežnika 451 4.7.0. Poskusite znova pozneje. PRX4 je večinoma začasen.« 

Prepričajte se, da ne uporabljate nabiralnika v skupni rabi za pošiljanje prek odjemalca SMTP, saj način pošiljanja prek odjemalca SMTP zahteva licenciran nabiralnik za pošiljanje pošte. Če pa nabiralnika v skupni rabi ne uporabljate in težave ne morete odpraviti, preverite to:

1. Za zagon tega ukaza PowerShell omogočite pošiljanje odjemalca SMTP v licenciranem nabiralniku:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    OR

    1. Pojdite na Skrbniško središče za Microsoft 365 > **aktivnih** uporabnikov in izberite uporabnika.
    1. Pojdite na zavihek Pošta, da > **e-poštne aplikacije** > izberite **Upravljanje e-poštnih aplikacij.** 
    1. Preverite, ali **je nastavitev SMTP s** preverjeno pristnostjo potrjena (omogočena).
    1. Izberite **Shrani spremembe.**
    
    Če želite omogočiti preverjanje pristnosti SMTP za celotno organizacijo, zaženite ta ukaz:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Opomba:** Iz varnostnih razlogov priporočamo, da preverjanje pristnosti SMTP omogočite le za nabiralnik, ki ga uporabljate. Nastavitev na ravni uporabnika preglasi nastavitev na ravni organizacije.

2. Privzete nastavitve varnosti Azure onemogočite tako, da možnosti Omogoči **privzete nastavitve nastavite** na **Ne:**

    1. V portal Azure se vpišite kot skrbnik za varnost, skrbnik pogojnega dostopa ali globalni skrbnik.
    1. Poiščite Azure Active Directory >lastnosti **  in** izberite **Upravljanje privzetih varnostnih nastavitev.**
    1. Nastavite **preklopni gumb Omogoči privzete varnostne** nastavitve na **Ne.**
    1. Izberite **Shrani**.

3. Onemogočite storitev Multi Factor Authentication (MFA) v licenciranem nabiralniku, ki se uporablja.

    1. Pojdite na Skrbniško središče za Microsoft 365 in v levem meniju za krmarjenje izberite **Uporabniki**  >  **aktivni uporabniki.**
    1. Na strani **Aktivni uporabniki** izberite **Multi-Factor Authentication.**
    1. Izberite uporabnika in onemogočite **večkratno preverjanje pristnosti.**

