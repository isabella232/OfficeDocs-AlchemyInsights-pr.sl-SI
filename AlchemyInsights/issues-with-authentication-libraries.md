---
title: Težave s knjižnicami za preverjanje pristnosti
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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063645"
---
# <a name="issues-with-authentication-libraries"></a>Težave s knjižnicami za preverjanje pristnosti

1. [Knjižnice za preverjanje pristnosti za Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) je na voljo za Microsoftove podprte in nezdružljive knjižnice odjemalca in vmesnega seznama.
2. Microsoftova knjižnica za preverjanje pristnosti (MSAL) podpira več [tokov preverjanja pristnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) za uporabo v različnih scenarijih programov.
3. Če želite preveriti pristnost in pridobiti žetone, inicializirate nov javni ali zaupen odjemalski program v kodi. Ko inicializirate odjemalski program v Microsoftovi knjižnici za preverjanje pristnosti (MSAL), lahko nastavite več možnosti konfiguracije. Če želite izvedeti več, glejte [možnosti konfiguracije aplikacije](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL) in Azure AD Graph API (graf ZVOČNIh grafikonov)**

Z **začetkom junija 30th 2020** ne bomo več dodali nobenih novih funkcij v knjižnice adal in Azure ad Graph. Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.

Z **začetkom junija 30th 2022** bomo zaključili podporo za knjižnice adal in Azure ad Graph in ne boste več zagotavljali tehnične podpore ali varnostnih posodobitev.

Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo *prejeli nobene tehnične podpore ali varnostnih posodobitev*.

Programi, ki uporabljajo Azure AD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne točke grafikona Azure AD.

**Selitev v knjižnice ADAL**

Priporočamo, da izvedete nadgradnjo na knjižnico [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki vključuje najnovejše funkcije in varnostne posodobitve.

Če uporabljate Microsoft apps, veste, da je Microsoft v postopku selitve svojih programov v MSAL z rokom za konec podpore, s čimer zagotovi, da bodo imeli koristi od trenutne varnosti in izboljšav funkcij v MSAL.

Za več informacij glejte:

1. [Preberite pogosta vprašanja o knjižnici ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Več informacij o selitvi aplikacij glede na platformo](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, vam priporočamo, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne ISVs ali ponudnike programov. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.

**Selitev zmogljivosti AAD Graph**

Za programe, ki uporabljajo grafiko Azure AD Graph, upoštevajte navodila za [selitev programov AZURE ad Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Naš kontrolni seznam selitve zagotavlja uvodno mesto.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph. Priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij. Microsoftova podpora vam omogoča tudi seznam vseh uporab ZVOČNIh grafikonov v najemniku.
3. Če želite za program dostopati do podatkov v programu Microsoft Graph, ga mora uporabnik ali skrbnik dodeliti pravilnim dovoljenjem prek postopka soglasja. [Sklici na dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) navajajo dovoljenja, povezana z vsakim glavnim naborom API-jev Microsoft Graph. Na voljo so tudi navodila za uporabo dovoljenj.
