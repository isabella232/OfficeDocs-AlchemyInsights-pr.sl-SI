---
title: Poizvedovanje po Microsoftovem Graph API-ja
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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923255"
---
# <a name="querying-the-microsoft-graph-api"></a>Poizvedovanje po Microsoftovem Graph API-ja

Ta tema lahko velja tudi za razvijalce, ki še vedno uporabljajo Azure AD Graph API. Vendar pa je zelo **priporočljivo, da** uporabite Microsoft Graph za vse scenarije za upravljanje imenika, identitete in dostopa.

**Težave s preverjanjem pristnosti ali pooblastilom**

- Če vaša  aplikacija ne more pridobiti žetonov za priklic storitve Microsoft Graph, izberite Težava z pridobivanjem žetona za dostop **(preverjanje pristnosti)** v kategoriji Microsoft Graph, da pridobite natančnejšo pomoč in podporo za to temo.
- Če je program pri klicu storitve Microsoft Graph prejel napake s pooblastilom **401 ali 403,** izberite kategorijo Pridobivanje napake s pooblastilom **za** Microsoft Graph API, da pridobite natančnejšo pomoč in podporo za to temo.

**Želim uporabljati Microsoft Graph, vendar ne vem, kje začeti**

Če želite izvedeti več o storitvi Microsoft Graph, glejte:

- [Pregled storitve Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled upravljanja identitet in dostopa v storitvi Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Uvod v izgradnjo Aplikacij Microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – preskusite MICROSOFTOVE Graph API-je v najemniku ali demonantu

**Želim uporabiti Microsoft Graph, vendar podpira API-je imenika v1.0, ki jih potrebujem?**

Microsoft Graph je priporočen API za upravljanje imenika, identitete in dostopa. Kljub temu pa obstaja še nekaj vrzeli med tem, kar je mogoče v storitvah Azure AD Graph in Microsoft Graph. Preglejte te članke, v katerih so poudarjene najbolj posodobljene razlike, s katerimi si lahko pomagate pri vaši izbiri:

- [Razlike med vrsto vira med imenikoma Azure AD Graph in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike med lastnostmi med imenikoma Azure AD Graph in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike med metodami med imenikoma Azure AD in Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Če poizvedem *po uporabniškem* predmetu, manjka veliko njegovih lastnosti**

`GET https://graph.microsoft.com/v1.0/users`vrne le 11 lastnosti, saj Graph Microsoft samodejno izbere privzeti nabor uporabniških *lastnosti,* ki jih bo vrnil. Če potrebujete druge *uporabniške lastnosti,* uporabite $select in izberite lastnosti, ki jih potrebujete za aplikacijo. Najprej preskusite v **Microsoft Graph Explorerju.**

**Nekatere vrednosti uporabniških lastnosti so *ničelne,* čeprav vem, da so nastavljene**

Najverjetnejša razlaga je, da je imela aplikacija dovoljenje *User.ReadBasic.All.* To aplikaciji omogoča, da prebere omejen nabor uporabniških lastnosti in vrne vse druge lastnosti kot ničelne vrednosti, tudi če so bile že nastavljene. Namesto tega odobrite *aplikacijo User.Read.All.*

Če želite več informacij, [glejte Dovoljenja Graph Microsoftu.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Pri uporabi parametrov poizvedbe OData za filtriranje podatkov v zahtevah imam težave**

Microsoft Graph podpira širok nabor parametrov poizvedbe OData, vendar imeniške storitve (viri, ki dedujejo od *imenikaObject)* v microsoft Graph v celoti ne podpirajo teh parametrov. Enake omejitve, ki so bile prisotne v imeniku Azure AD Graph v Microsoft Graph:

1. **Ni podprto:**$count, $search in $filter ničelne *ali* *ničelne* vrednosti
2. **Ni podprto:**$filter določenih lastnostih (glejte teme o virih, za katere so lastnosti mogoče filtrirati)
3. **Ni podprto:** ostranitev, filtriranje in razvrščanje hkrati
4. **Ni podprto:** filtriranje relacije. Poiščite na primer vse člane inženirske skupine, ki so v Združenem kraljestvu.
5. **Delna** podpora: $orderby *uporabnika* (samo prikazanoIme in uporabniškoImeU šablone) in *skupine*
6. **Delna** podpora: $filter (podpira le eq *,* *startswith* *ali*, and , *and*, and limited *any*) podporo za $expand (razširjanje relacij enega predmeta vrne vse relacije, vendar je razširitev zbirke relacij predmetov omejena)

Če želite več informacij, glejte [Prilagajanje odgovorov s parametri poizvedbe.](https://docs.microsoft.com/graph/query-parameters)

**API, ki ga kličem, ne deluje – kje lahko preskusim več?**

**Microsoft Graph Explorer** – preskusite API Graph Microsoft Graph najemniku ali demonantu in  si oglejte vzorčne poizvedbe v Microsoft Graph Explorerju.

**Ko poizvedim po podatkih, se zdi, da dobim nepopolni nabor podatkov**

Če želite s poizvedbo po zbirki (kot so *uporabniki),* Microsoft Graph uporablja omejitve strani na strani strežnika, tako da so rezultati vedno vrnjeni s privzeto velikostjo strani. Za vašo aplikacijo bi moralo biti vedno pričakovano, da bo prestala vse zbirke, ki ste jih vrnili iz storitve.

Če želite več informacij, si oglejte:

- [Najboljše prakse Graph Microsoftu](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph data in your app](https://docs.microsoft.com/graph/paging)

**Moja aplikacija je prepočasna in je tudi dušena. Katere izboljšave lahko naredim?**

Glede na vaš scenarij so na voljo številne različne možnosti, s tem pa poskrbite, da bo vaša aplikacija bolj učinkovitejša in v nekaterih primerih s storitvijo manjša (če opravljate preveč klicev).

Več informacij nadete v tem članku:

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
