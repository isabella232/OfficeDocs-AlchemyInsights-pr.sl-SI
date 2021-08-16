---
title: Težave s knjižnicami preverjanja pristnosti
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028020"
---
# <a name="issues-with-authentication-libraries"></a>Težave s knjižnicami preverjanja pristnosti

1. [Microsoftova platforma za identitete knjižnice za preverjanje pristnosti](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) naštejejo Microsoftove knjižnice, ki so podprte in združljive z odjemalcem in programsko opremo.
2. Microsoftova knjižnica preverjanja pristnosti (MSAL) podpira več [tokov](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) preverjanja pristnosti, ki jih lahko uporabite v različnih scenarijih aplikacije.
3. Če želite preveriti pristnost in pridobiti žetone, v kodi inicializirate novo javno ali zaupno odjemalsko aplikacijo. Ko inicializirate odjemalski program v Microsoftovi knjižnici preverjanja pristnosti (MSAL), lahko nastavite več možnosti konfiguracije. Če želite izvedeti več, glejte [Možnosti konfiguracije aplikacije.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Konec podpore za knjižnico za preverjanje Azure Active Directory pristnosti (ADAL) in Azure AD Graph API (AAD Graph)**

**Od 30. junija 2020** ne bomo več dodajali novih funkcij v ADAL in Azure AD Graph. Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.

**Od 30. junija 2022** se bo končala podpora za ADAL in Azure AD Graph in ne bomo več zagotavljali tehnične podpore ali varnostnih posodobitev.

Aplikacije, ki uporabljajo ADAL v obstoječih različicah operacijskega sistema, bodo po tem času še naprej delovale, vendar ne bodo dobile nobenih tehničnih posodobitev *za podporo ali varnostnih posodobitev.*

Aplikacije, ki uporabljajo Azure AD Graph po tem času morda ne bodo več prejemali odgovorov iz končne točke Graph Azure AD.

**Selitev ADAL**

Priporočamo, da izvedete nadgradnjo na knjižnico [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki vključuje najnovejše funkcije in varnostne posodobitve.

Če uporabljate Microsoftove aplikacije, veste, da Microsoft do konca obdobja podpore izvaja selitev svojih aplikacij v MSAL, kar jim zagotavlja, da jim bo koristila stalna varnost in izboljšave funkcij MSAL.

Če želite več informacij, si oglejte:

1. [Preberite pogosta vprašanja o knjižnici ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Več informacij o selitvi aplikacij glede na platformo](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Če potrebujete pomoč pri razumevanju, katero od aplikacij uporabljate ADAL, vam priporočamo, da pregledate izvorno kodo vseh aplikacij in se, če je na voljo, preglejte morebitne ponudnike internetnih storitev ali ponudnike aplikacij. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.

**Selitev zmogljivosti AAD Graph**

Za aplikacije, ki uporabljajo Azure AD Graph, upoštevajte naša navodila za selitev [aplikacij Azure AD Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Naš kontrolni seznam selitve zagotavlja točko za začetek.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph. Priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij. Microsoftova podpora vam lahko zagotovi tudi seznam vseh AAD-Graph uporabe v vašem najemniku.
3. Če želite, da vaša aplikacija dostopa do podatkov v Graph Microsoft Graph, ji mora uporabnik ali skrbnik prek postopka podelitve soglasja podeliti ustrezna dovoljenja. V [sklicu Graph Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) navedeni dovoljenji, ki so povezana z vsakim glavnim naborom API-jev Graph Microsoft Graph. V njem so na voljo tudi navodila za uporabo dovoljenj.
