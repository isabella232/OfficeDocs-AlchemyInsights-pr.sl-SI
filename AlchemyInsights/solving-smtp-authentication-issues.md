---
title: Omogočanje preverjanja pristnosti in odpravljanja težav SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 14f1454ad687b4d76cf419583b442685fa19b5a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321769"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>Omogočanje preverjanja pristnosti in odpravljanja težav SMTP

Če želite omogočiti preverjanje pristnosti SMTP za nabiralnik ali pa se prikaže napaka »Odjemalec ni preverjen«, »Preverjanje pristnosti neuspešno« ali »SmtpClientAuthentication« s kodo 5.7.57 ali 5.7.3 ali 5.7.139, ko poskušate posredovati e-pošto s preverjanjem pristnosti naprave ali aplikacije s protokolom Microsoft 365, izvedite ta tri dejanja, da odpravite težavo:

1. Privzete nastavitve [varnosti Azure onemogočite tako,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) da možnost Omogoči **privzete nastavitve nastavite** na **Ne.**

    a. V portal Azure se vpišite kot skrbnik za varnost, skrbnik pogojnega dostopa ali globalni skrbnik.<BR/>
    b. Poiščite Azure Active Directory > **lastnosti.**<BR/>
    c. Izberite **Upravljanje privzetih varnostnih nastavitev.**<BR/>
    d. Nastavite **Omogoči privzete varnostne nastavitve** na **Ne.**<BR/>
    e. Izberite **Shrani**.

2. [Omogočanje pošiljanja SMTP odjemalca](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) v licenciranem nabiralniku.

    a. V Skrbniško središče za Microsoft 365 izberite **aktivni uporabniki** in izberite uporabnika.<BR/>
    b. Pojdite na zavihek Pošta in v razdelku **E-poštne aplikacije** izberite Upravljanje **e-poštnih aplikacij**.<BR/>
    d. Preverite, **ali je potrjeno polje SMTP s** preverjeno pristnostjo (omogočeno).<BR/>
    e. Izberite **Shrani spremembe.**<BR/>

3. [Onemogočite storitev Multi-Factor Authentication (MFA) v](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) licenciranem nabiralniku.

    a. Pojdite na Skrbniško središče za Microsoft 365 in v levem meniju za krmarjenje **izberite** Uporabniki  >  **aktivni uporabniki.**<BR/>
    b. Izberite **Multi-Factor Authentication**.<BR/>
    c. Izberite uporabnika in onemogočite **Multi-Factor auth.**<BR/>
