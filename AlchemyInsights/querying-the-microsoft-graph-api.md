---
title: Poizvedovanje po API-ju Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974686"
---
# <a name="querying-the-microsoft-graph-api"></a>Poizvedovanje po API-ju Microsoft Graph

Ta tema se lahko uporablja tudi za razvijalce, ki še vedno uporabljajo vmesnik Azure AD Graph API. Vendar pa **je priporočljivo,** da uporabite Microsoft Graph za vse scenarije imenika, identitete in upravljanja Accessa.

**Težave s preverjanjem pristnosti ali avtorizacije**

- Če vaš program **ne more pridobiti žetonov** za klicanje programa Microsoft Graph, izberite **težave z iskanjem žetona Microsoft Graph (preverjanje pristnosti)** , da pridobite natančnejšo pomoč in podporo v tej temi.
- Če vaš program **prejema napake pri avtorizaciji v storitvi 401 ali 403** , ko kličete Microsoft Graph, izberite kategorijo» **pridobivanje zavrnjenega dostopa «(avtorizacija)** , ki je v kategoriji API za Microsoft Graph, da pridobite natančnejšo pomoč in podporo v tej temi.

**Želim uporabljati Microsoft Graph, vendar ne vem, kje naj začnem**

Če želite izvedeti več o programu Microsoft Graph, glejte:

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled identitete in upravljanja dostopa v programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Uvod v izgradnjo aplikacij Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – preskusite API-je za Microsoft Graph v najemniku ali v demonstracijskem najemniku

**Želim uporabiti Microsoft Graph, vendar ne podpira API-jev imenika v 1.0, ki jih potrebujem?**

Microsoft Graph je priporočen API za imenik, identiteto in upravljanje dostopa. Vendar pa še vedno obstaja nekaj vrzeli med tem, kar je mogoče v storitvi Azure AD Graph in Microsoft Graph. Preglejte te članke, ki poudarjajo najbolj posodobljene razlike, ki jih boste lažje izbrali:

- [Razlike med vrstami virov med grafikonom Azure AD Graph in programom Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike med lastnostmi in grafikoni za Azure AD Graph in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike v metodi med storitvijo Azure AD in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Ko poizvedujem po predmetu *uporabnika* , manjkajo številne njegove lastnosti**

`GET https://graph.microsoft.com/v1.0/users` vrne le 11 lastnosti, saj Microsoft Graph samodejno izbere privzeti nabor *uporabniških* lastnosti za vrnitev. Če potrebujete druge lastnosti *uporabnika* , uporabite $SELECT, da izberete lastnosti, ki jih potrebuje vaš program. Najprej preskusite v **programu Microsoft Graph Explorer** .

**Nekatere vrednosti lastnosti uporabnika so *ničelne* , čeprav vem, da so nastavljene**

Najbolj verjetna razlaga je, da je bila aplikacija dodeljena *uporabniku. ReadBasic. vse* dovoljenje. S tem lahko program prebere omejen nabor uporabniških lastnosti, vrne vse druge lastnosti kot NULL, tudi če so bile prej nastavljene. Poskusite podeliti *uporabnika aplikacije. preberi. vse* dovoljenje namesto tega.

Če želite več informacij, glejte [uporabniška dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Imam težave z uporabo parametrov poizvedbe OData za filtriranje podatkov v mojih zahtevah**

Medtem ko Microsoft Graph podpira širok spekter parametrov OData poizvedbe, številni od teh parametrov niso v celoti podprti s imeniškimi storitvami (viri, ki dedujejo od *directoryObject*) v programu Microsoft Graph. Enake omejitve, ki so bile predstavljene v grafu Azure AD, se večinoma pojavljajo v programu Microsoft Graph:

1. **Ni podprto**: $count, $search in *$filter v vrednosti null* ali *NOT NULL*
2. **Ni podprto**: $filter v določenih lastnostih (glejte teme vira, ki jih je treba filtrirati)
3. **Ni podprto**: ostranjevanje, filtriranje in razvrščanje hkrati
4. **Ni podprto**: filtriranje v relaciji. Na primer – poiščite vse člane inženirske skupine, ki so v Združenem kraljestvu.
5. **Delna podpora**: $OrderBy na *uporabnika* (le displayName in userPrincipalName) in *skupino*
6. **Delna podpora**: $filter (podpira *le EQ*, *startswith*, or *in Limited* *) podpora*, $Expand (razširitev relacije posameznega predmeta vrne vse relacije, vendar pa je razširitev zbirke predmetov» relacija «omejena) 

Če želite več informacij, glejte [prilagajanje odgovorov s parametri poizvedbe](https://docs.microsoft.com/graph/query-parameters).

**Klic API, ki ga kličem, ne deluje – kje lahko naredim več testiranj?**

**Microsoft Graph Explorer** – preskusite API-je za Microsoft Graph v najemnika ali demonstracijskega najemnika in preverite **vzorčne poizvedbe** v Raziskovalcu programa Microsoft Graph.

**Ko poiščem podatke, se zdi, kot da dobim nedokončan nabor podatkov**

Če poizvedujete po zbirki (kot so *Uporabniki*), Microsoft Graph uporabi omejitve strani strežnika, tako da so rezultati vedno vrnjeni s privzeto velikostjo strani. Program mora vedno pričakovati, da se bo stran povrnila prek zbirk, vrnjenih iz storitve.

Za več informacij glejte:

- [Najboljše prakse v programu Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Ostranjevanje podatkov v aplikaciji Microsoft Graph](https://docs.microsoft.com/graph/paging)

**Aplikacija je prepočasna in je tudi zadaviti. Katere izboljšave lahko izvedem?**

Odvisno od vašega scenarija je na voljo več različnih možnosti, s katerimi lahko izboljšate svojo aplikacijo in v nekaterih primerih zmanjšate možnost za omejevanje storitve (ko vnašate preveč klicev).

Več informacij nadete v tem članku:

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
