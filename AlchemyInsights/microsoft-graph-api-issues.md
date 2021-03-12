---
title: Težave z API-jem za Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714514"
---
# <a name="microsoft-graph-api-issues"></a>Težave z API-jem za Microsoft Graph

Ta tema se lahko uporablja tudi za razvijalce, ki še vedno uporabljajo vmesnik Azure AD Graph API. Vendar pa **je priporočljivo,** da uporabite Microsoft Graph za vse scenarije imenika, identitete in upravljanja Accessa.

**Težave s preverjanjem pristnosti ali avtorizacije**

- Če vaš program **ne more pridobiti žetonov** za klicanje programa Microsoft Graph, izberite **težave z iskanjem žetona Microsoft Graph (preverjanje pristnosti)** , da pridobite natančnejšo pomoč in podporo v tej temi.
- Če vaš program **prejema napake pri avtorizaciji v storitvi 401 ali 403** , ko kličete Microsoft Graph, izberite kategorijo» **pridobivanje zavrnjenega dostopa «(avtorizacija)** , ki je v kategoriji API za Microsoft Graph, da pridobite natančnejšo pomoč in podporo v tej temi.

**Želim uporabljati Microsoft Graph, vendar ne vem, kje naj začnem**

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled identitete in upravljanja dostopa v programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Uvod v izgradnjo aplikacij Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – preskusite API-je za Microsoft Graph v najemniku ali v demonstracijskem najemniku

**Želim uporabiti Microsoft Graph, vendar ne podpira API-jev imenika v 1.0, ki jih potrebujem?**

Microsoft Graph je priporočen API za imenik, identiteto in upravljanje dostopa. Vendar pa še vedno obstaja nekaj vrzeli med tem, kar je mogoče v storitvi Azure AD Graph in Microsoft Graph. Preglejte te članke, ki poudarjajo najbolj posodobljene razlike, ki jih boste lažje izbrali:

- [Razlike med vrstami virov med grafikonom Azure AD Graph in programom Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike med lastnostmi in grafikoni za Azure AD Graph in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike v metodi med storitvijo Azure AD in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, ki jo kličem, ne deluje – kje lahko naredim več testiranj?**

**Microsoft Graph Explorer** – preskusite API-je za Microsoft Graph v najemnika ali demonstracijskega najemnika in preverite **vzorčne poizvedbe** v Raziskovalcu programa Microsoft Graph.

**Aplikacija je prepočasna in je tudi zadaviti. Katere izboljšave lahko izvedem?**

Odvisno od vašega scenarija je na voljo več možnosti, s katerimi lahko izboljšate svojo aplikacijo in v nekaterih primerih manj nagnjeni k omejevanju storitve (ko vnašate preveč klicev).

- [Najboljše prakse v programu Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Zahteve za betonarne](https://docs.microsoft.com/graph/json-batching)
- [Sledenja spremembam prek poizvedbe Delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Pridobivanje obvestil o spremembah s pomočjo](https://docs.microsoft.com/graph/webhooks)
- [Usmerjanje zadaviti](https://docs.microsoft.com/graph/throttling)

**Kje lahko najdem več informacij o napakah in znanih težavah?**

- [Informacije o odgovoru na Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Znane težave z Microsoft Graphom](https://docs.microsoft.com/graph/known-issues)

**Kje lahko preverim stanje razpoložljivosti storitve in povezljivosti?**

Razpoložljivost storitve in povezljivost osnovnih storitev, do katerih lahko dostopate prek Microsoft Grapha, lahko vpliva na splošno razpoložljivost in učinkovitost delovanja programa Microsoft Graph.

- Za zdravje storitve Azure Active Directory preverite stanje storitve **Security + Identity** Services, ki so navedene na [strani stanja Azure](https://azure.microsoft.com/status/).
- Za Officeove storitve, ki prispevajo k programu Microsoft Graph, preverite stanje storitev, ki so navedene v [nadzorni plošči» zdravstvena služba za Office](https://portal.office.com/adminportal/home#/servicehealth)«.

Napake pri avtorizaciji za Microsoft Graph so lahko posledica več različnih težav, od katerih večina ustvari napako 401 ali 403. To lahko na primer privede do napak pri avtorizaciji:

- Napačni [poteki pridobivanja žetona za dostop](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Neustrezno konfigurirani [obsegi dovoljenja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Manjkajoče [soglasje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Konec podpore za knjižnico Azure Active Directory Authentication Library (ADAL) in vmesnik API za Azure AD Graph (AAD Graph)_* _

_ * Začetek junija 30th, 2020 * *, ne bomo več dodali nobenih novih funkcij v knjižnice ADAL in Azure AD Graph. Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.

Z **začetkom junija 30th 2022** bomo zaključili podporo za knjižnice adal in Azure ad Graph in ne boste več zagotavljali tehnične podpore ali varnostnih posodobitev.

Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo *prejeli nobene tehnične podpore ali varnostnih posodobitev*.

Programi, ki uporabljajo Azure AD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne točke grafikona Azure AD.

**Selitev v knjižnice ADAL**

Priporočamo, da izvedete nadgradnjo na knjižnico [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki vključuje najnovejše funkcije in varnostne posodobitve.

Če uporabljate Microsoft apps, veste, da je Microsoft v postopku selitve svojih programov v MSAL s končnim rokom za konec podpore, s čimer zagotovite, da bodo imeli koristi od trenutne varnosti in izboljšav funkcij v MSAL.

1. [Preberite pogosta vprašanja o knjižnici ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Več informacij o selitvi aplikacij glede na platformo](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, vam priporočamo, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne ISVs ali ponudnike programov. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.

**Selitev zmogljivosti AAD Graph**

Za programe, ki uporabljajo grafiko Azure AD Graph, upoštevajte navodila za [selitev programov AZURE ad Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Kontrolni seznam za selitev vključuje točko za začetek izvajanja postopka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph. Priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij. Microsoftova podpora vam omogoča tudi seznam vseh uporab ZVOČNIh grafikonov v najemniku.
3. Če želite za program dostopati do podatkov v programu Microsoft Graph, ga mora uporabnik ali skrbnik dodeliti pravilnim dovoljenjem prek postopka soglasja. [Sklici na dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) navajajo dovoljenja, povezana z vsakim glavnim naborom API-jev Microsoft Graph. Na voljo so tudi navodila za uporabo dovoljenj.
