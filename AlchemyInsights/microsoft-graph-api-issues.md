---
title: Težave z api Graph Microsoft Graph Microsoft
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
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975909"
---
# <a name="microsoft-graph-api-issues"></a>Težave z api Graph Microsoft Graph Microsoft

Ta tema lahko velja tudi za razvijalce, ki še vedno uporabljajo Azure AD Graph API. Vendar pa je zelo **priporočljivo, da** uporabite Microsoft Graph za vse scenarije za upravljanje imenika, identitete in dostopa.

**Težave s preverjanjem pristnosti ali pooblastilom**

- Če vaša  aplikacija ne more pridobiti žetonov za priklic storitve Microsoft Graph, izberite Težava z pridobivanjem žetona za dostop **(preverjanje pristnosti)** v kategoriji Microsoft Graph, da pridobite natančnejšo pomoč in podporo za to temo.
- Če je program pri klicu storitve Microsoft Graph prejel napake s pooblastilom **401 ali 403,** izberite kategorijo Pridobivanje napake s pooblastilom **za** Microsoft Graph API, da pridobite natančnejšo pomoč in podporo za to temo.

**Želim uporabljati Microsoft Graph, vendar ne vem, kje začeti**

- [Pregled storitve Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled upravljanja identitet in dostopa v storitvi Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Uvod v izgradnjo Aplikacij Microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – preskusite MICROSOFTOVE Graph API-je v najemniku ali demonantu

**Želim uporabiti Microsoft Graph, vendar podpira API-je imenika v1.0, ki jih potrebujem?**

Microsoft Graph je priporočen API za upravljanje imenika, identitete in dostopa. Kljub temu pa obstaja še nekaj vrzeli med tem, kar je mogoče v storitvah Azure AD Graph in Microsoft Graph. Preglejte te članke, v katerih so poudarjene najbolj posodobljene razlike, s katerimi si lahko pomagate pri vaši izbiri:

- [Razlike med vrsto vira med imenikoma Azure AD Graph in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike med lastnostmi med imenikoma Azure AD Graph in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike med metodami med imenikoma Azure AD in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, ki ga kličem, ne deluje – kje lahko preskusim več?**

**Microsoft Graph Explorer** – preskusite API Graph Microsoft Graph najemniku ali demonantu in  si oglejte vzorčne poizvedbe v Microsoft Graph Explorerju.

**Moja aplikacija je prepočasna in je tudi dušena. Katere izboljšave lahko naredim?**

Glede na vaš scenarij so na voljo številne možnosti, s katerih bo vaša aplikacija bolj učinkovitejša in v nekaterih primerih manjša, kot če je storitev manjša (če opravljate preveč klicev).

- [Najboljše prakse Graph Microsoftu](https://docs.microsoft.com/graph/best-practices-concept)
- [Zahteve za paketiranje](https://docs.microsoft.com/graph/json-batching)
- [Sledenje spremembam s poizvedbo delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Get notified of changes through webhooks](https://docs.microsoft.com/graph/webhooks)
- [Smernice za dušenje](https://docs.microsoft.com/graph/throttling)

**Kje lahko najdem več informacij o napakah in znanih težavah?**

- [Informacije o Graph o napakah v aplikaciji Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Znane težave s storitvijo Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kje lahko preverim stanje razpoložljivosti storitve in povezljivosti?**

Razpoložljivost storitve in povezljivost temeljnih storitev, do katerih lahko dostopate prek storitve Microsoft Graph, lahko vplivajo na splošno razpoložljivost in učinkovitost delovanja storitve Microsoft Graph.

- Če Azure Active Directory podatkov o stanju storitve, preverite stanje storitev **Varnost + identiteta,** ki so navedene na [strani Stanje storitve Azure.](https://azure.microsoft.com/status/)
- Če Office storitve, ki prispevajo k storitvi Microsoft Graph, preverite stanje storitev, ki so navedene na [nadzorni plošči Office stanje storitve](https://portal.office.com/adminportal/home#/servicehealth).

Napake Graph microsofta so lahko posledica več različnih težav, od katerih je večina ustvarila napako 401 ali 403. Na primer, vse to lahko povzroči napake pri avtorizacijah:

- Napačni [poteki pridobivanja žetona za dostop](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Neustrezno konfigurirani [obsegi dovoljenja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Manjkajoče [soglasje](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Konec podpore za knjižnico za preverjanje Azure Active Directory pristnosti (ADAL) in Azure AD Graph API (AAD Graph)***

**Od 30. junija 2020** ne bomo več dodajali novih funkcij v ADAL in Azure AD Graph. Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.

**Od 30. junija 2022** se bo končala podpora za ADAL in Azure AD Graph in ne bomo več zagotavljali tehnične podpore ali varnostnih posodobitev.

Aplikacije, ki uporabljajo ADAL v obstoječih različicah operacijskega sistema, bodo po tem času še naprej delovale, vendar ne bodo dobile nobenih tehničnih posodobitev *za podporo ali varnostnih posodobitev.*

Aplikacije, ki uporabljajo Azure AD Graph po tem času morda ne bodo več prejemali odgovorov iz končne točke Graph Azure AD.

**Selitev ADAL**

Priporočamo, da izvedete nadgradnjo na knjižnico [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki vključuje najnovejše funkcije in varnostne posodobitve.

Če uporabljate Microsoftove aplikacije, veste, da Microsoft do konca roka za podporo izvaja selitev svojih aplikacij v MSAL, pri čemer jim zagotavlja, da bo izkoristil prednosti trenutnih izboljšav MSAL, ki stalno izboljšujejo varnost in funkcije.

1. [Preberite pogosta vprašanja o knjižnici ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Več informacij o selitvi aplikacij glede na platformo](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Če potrebujete pomoč pri razumevanju, katero od aplikacij uporabljate ADAL, vam priporočamo, da pregledate izvorno kodo vseh aplikacij in se, če je na voljo, preglejte morebitne ponudnike internetnih storitev ali ponudnike aplikacij. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.

**Selitev zmogljivosti AAD Graph**

Za aplikacije, ki uporabljajo Azure AD Graph, upoštevajte naša navodila za selitev [aplikacij Azure AD Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Kontrolni seznam za selitev vključuje točko za začetek izvajanja postopka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph. Priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij. Microsoftova podpora vam lahko zagotovi tudi seznam vseh AAD-Graph uporabe v vašem najemniku.
3. Če želite, da vaša aplikacija dostopa do podatkov v Graph Microsoft Graph, ji mora uporabnik ali skrbnik prek postopka podelitve soglasja podeliti ustrezna dovoljenja. V [sklicu Graph Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) navedeni dovoljenji, ki so povezana z vsakim glavnim naborom API-jev Graph Microsoft Graph. V njem so na voljo tudi navodila za uporabo dovoljenj.
