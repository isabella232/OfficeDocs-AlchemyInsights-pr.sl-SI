---
title: Težave s preverjanjem pristnosti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976865"
---
# <a name="authentication-issues"></a>Težave s preverjanjem pristnosti

**Ali želite pridobiti informacije o kodah napak AADSTS, ki jih vrne storitev varnostnih žetonov (STS) Azure Active Directory (Azure AD)?** Za opise napak AADSTS, popravke in predlagane rešitve glejte razdelek [Kode napak preverjanja pristnosti in avtorizacije storitve Azure AD](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes).

Vzrok za napake avtorizacije so lahko različne težave – večina težav javi napako 401 ali 403. Napake avtorizacije lahko na primer javijo spodnje težave:

- Napačni [poteki pridobivanja žetona za dostop](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Neustrezno konfigurirani [obsegi dovoljenja](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Manjkajoče [soglasje](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Če želite odpraviti običajne napake avtorizacije, poskusite izvesti spodnje korake, ki najbolj ustrezajo prejeti napaki. Za prejeto napako lahko velja več korakov.

**Napaka »401 Nepooblaščeno«: Ali je vaš žeton veljaven?**

Prepričajte se, da aplikacija uporablja veljaven žeton za dostop do vmesnika Microsoft Graph kot del zahteve. Ta napaka običajno pomeni, da v glavi zahteve za preverjanje pristnosti HTTP manjka žeton za dostop ali pa žeton ni veljaven oziroma je potekel. Za pridobivanje žetona za dostop priporočamo uporabo knjižnice Microsoft Authentication Library (MSAL). Do te napake lahko pride tudi, če želite uporabiti žeton za pooblaščen dostop, odobren za osebni Microsoftov račun za dostop do vmesnika API, ki podpira le službene ali šolske račune (računi organizacije).

**Napaka »403 Prepovedano«: Ali ste izbrali ustrezen nabor dovoljenj?**

Prepričajte se, da ste zahtevali ustrezen nabor dovoljenj, glede na vmesnike API za Microsoft Graph, ki jih prikliče aplikacija. Priporočena dovoljenja za dostop z minimalnimi pravicami so na voljo za vse teme referenčnih načinov vmesnika API za Microsoft Graph. Ta dovoljenja mora za aplikacijo odobriti uporabnika ali skrbnik. Postopek odobritve dovoljenj je običajno izveden na strani za soglasje ali z uporabo lista za registracijo aplikacije na portala Azure. Na listu **Nastavitve** za aplikacijo kliknite **Zahtevana dovoljenja**, nato pa kliknite **Odobri dovoljenja**. Za več informacij glejte:

- [Dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dovoljenj in soglasja za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Napaka »403 Prepovedano«: Ali je aplikacija pridobila žeton, ki ustreza izbranim dovoljenjem?**

Prepričajte se, da se vrste zahtevanih ali odobrenih dovoljenj ujemajo z vrsto žetona za dostop, ki ga je pridobila aplikacija. Morda ste zahtevali ali odobrili dovoljenja za aplikacijo, uporabljate pa žetone za tok pooblaščene interaktivne kode namesto žetonov za tok poverilnic odjemalca ali pa ste zahtevali in odobrili pooblaščena dovoljenja, uporabljate pa žetone za tok poverilnic odjemalca namesto žetonov za tok pooblaščene kode.

Za več informacij o pridobivanju tokov glejte:

- [Pridobivanje dostopa v imenu uporabnikov in pooblaščenih dovoljenj](https://docs.microsoft.com/graph/auth-v2-user) 
- [Tok avtorizacijske kode Azure AD v2.0 - OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pridobivanje dostopa brez uporabnika (storitev strežniškega procesa) in dovoljenj za aplikacijo](https://docs.microsoft.com/graph/auth-v2-service) 
- [Tok poverilnic odjemalca Azure AD v2.0 - OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Napaka »403 Prepovedano«: ponastavitev gesla**

Trenutno ni nobenega strežniškega procesa za dovoljenja »od storitve do storitve« za aplikacijo, ki omogočajo ponastavitev gesel. Ti vmesniki API so podprti le za uporabo tokov interaktivne pooblaščene kode z vpisanim skrbnikom. Za več informacij glejte [Dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**»403 Prepovedano«: Ali ima uporabnik dostop in ustrezno licenco?**

Za toke pooblaščene kode Microsoft Graph oceni, ali je bila zahteva dovoljena, glede na odobrena dovoljenja za aplikacijo ter vrsto dovoljenj vpisanega uporabnika. Ta napaka običajno označuje, da uporabnik nima prednostnih dovoljenj za izvajanje zahteve **ali** pa nima licence za dostop do podatkov. Zahtevo lahko uspešno izvedejo le uporabniki z zahtevanimi dovoljenji ali licencami.

**»403 Prepovedano«: Ali ste izbrali pravilen vmesnik API vira?**

Storitve API, kot je Microsoft Graph, preverijo, ali se zahteva *občinstva* v prejetem žetonu za dostop ujema s pričakovano vrednostjo. Če temu ni tako, je javljena napaka »403 Prepovedano«. Običajno do te napake pride, ker poskušate uporabiti žeton, pridobljen za vmesnike API za Azure AD Graph, vmesnike API za Outlook ali vmesnike API za SharePoint/OneDrive, da bi priklicali Microsoft Graph (ali obratno). Zagotovite da se vir (ali obseg), za katerega aplikacija želi pridobiti žeton, ujema z vmesnikom API, ki ga aplikacija želi priklicati.

**»400 Neprimerna zahteva« ali »403 Prepovedano«: Ali uporabnik deluje v skladu s pravilnikom o pogojnem dostopu organizacije?**

Glede na pravilnike o pogojnem dostopu organizacije mora uporabnik, ki dostopa do virov vmesnika Microsoft Graph v aplikaciji, morda posredovati dodatne informacije, ki niso na voljo v žetonu za dostop, ki ga je aplikacija izvorno pridobila. V tem primeru je v aplikaciji javljena napaka **400 *zahtevana_interakcija*** med pridobivanjem žetona za dostop ali pa napaka **403 *nezadostne_zahteve*** med izvajanjem postopka klicanja vmesnika Microsoft Graph. V obeh primerih odgovor na napako vključuje dodatne informacije, ki jih je mogoče posredovati pooblaščeni končni točki, ki od uporabnika zahteva dodatne informacije (kot je večkratno preverjanje pristnosti ali včlanitev naprave).

Za več informacij o pogojnem dostopu glejte:

- [Obravnavanje težav s pogojnim dostopom s knjižnico MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Navodila za razvijalce za pogojni dostop za Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Konec podpore za knjižnico Azure Active Directory Authentication Library (ADAL) in vmesnik API za Azure AD Graph (AAD Graph)_* _

- Od 30. junija 2020 ne dodajamo več novih funkcij v knjižnico Azure Active Directory Authentication Library (ADAL) in vmesnik API za Azure AD Graph (AAD Graph). Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.
- 30. junija 2022 se je končala podpora za ADAL in AAD Graph, prav tako ni več na voljo tehnična podpora in varnostne posodobitve.
    - Aplikacije, ki uporabljajo ADAL v obstoječih različicah operacijskega sistema, bodo po tem obdobju še naprej delovale, vendar zanje ne bo več mogoče pridobiti tehnične podpore ali varnostnih posodobitev.
    - Aplikacije, ki uporabljajo AAD Graph, po tem obdobju morda ne bodo več prejemale odgovorov iz končne točke za AAD Graph.

_ *Selitev knjižnice ADAL**

Priporočamo, da izvedete nadgradnjo na knjižnico [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki vključuje najnovejše funkcije in varnostne posodobitve. To priporočilo je skladno s kontekstom selitve Microsoftovih aplikacij v knjižnico MSAL do roka za končanje podpore. Cilj selitve Microsoftovih aplikacij v knjižnico MSAL je zagotoviti aplikacijam prednosti rednih varnostnih in funkcijskih izboljšav knjižnice MSAL.

- [Preberite pogosta vprašanja o knjižnici ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Več informacij o selitvi aplikacij glede na platformo](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Če želite pomoč pri razumevanju, katere aplikacije uporabljajo knjižnico ADAL, priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij. Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.

**Selitev zmogljivosti AAD Graph**

Za aplikacije, ki uporabljajo AAD Graph, upoštevajte navodila za [selitev aplikacij Azure AD Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Kontrolni seznam za selitev vključuje točko za začetek izvajanja postopka](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph. Priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij. Microsoftova podpora vam lahko posreduje informacije o vseh uporabah zmogljivosti AAD Graph v vašem najemniku.

 










