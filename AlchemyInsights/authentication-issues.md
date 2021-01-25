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
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974791"
---
# <a name="authentication-issues"></a>Težave s preverjanjem pristnosti

**Iščete informacije o AADSTS kodah napak, ki so bile vrnjene v storitvi za varnost žetona Azure Active Directory ("Azure AD)" (STS)?** Če želite poiskati AADSTS opise napak, popravke in nekatere predlagane rešitve, glejte [kode napak za preverjanje pristnosti in avtorizacije AZURE ad](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) .

Napake pri avtorizaciji so lahko rezultat več različnih težav, od katerih večina ustvari napako 401 ali 403. Te težave lahko na primer privedejo do napak pri avtorizaciji:

- Nepravilni [tokovi za pridobitev žetona](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Slabo konfigurirani [obsegi dovoljenj](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Pomanjkanje [soglasja](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Če želite odpraviti pogoste napake avtorizacije, upoštevajte spodnja navodila, ki se najbolj ujemajo z napako, ki jo prejemate. Za napako, ki jo prejemate, lahko zaprosi več kot en korak.

- **nepooblaščena Napaka 401: ali je žeton veljaven?**

Zagotovite, da vaš program predstavlja veljaven žeton za dostop v Microsoft Graph kot del zahteve. Ta napaka pogosto pomeni, da žeton za dostop morda manjka v glavi zahteve za preverjanje pristnosti HTTP ali da je žeton neveljaven ali pa je potekel. Toplo priporočamo, da uporabite Microsoftovo knjižnico za preverjanje pristnosti (MSAL) za pridobitev žetona za dostop. Poleg tega lahko pride do te napake, če poskušate za dostop do API-ja, ki podpira le službene ali šolske račune (organizacijske račune), dodeliti žeton za pooblaščen dostop, ki je dodeljen osebnim Microsoftovim računom.

**403 prepovedana napaka: ali ste izbrali pravi nabor dovoljenj?**

Prepričajte se, da ste zahtevali pravilen nabor dovoljenj, ki temeljijo na programu Microsoft Graph API-ji za klice aplikacije. Priporočena najmanj privilegirana dovoljenja so na voljo v vseh temah referenčne metode za Microsoft Graph API. Poleg tega morajo ta dovoljenja odobriti aplikacija uporabnik ali skrbnik. Dodeljevanje dovoljenj se običajno zgodi prek privolitvene strani ali uporabe rezila za registracijo aplikacije Azure portal. Iz rezila z **nastavitvami** za aplikacijo kliknite **zahtevana dovoljenja** in nato še **dodeli dovoljenja**. Za več informacij glejte:

- [Dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dovoljenj in soglasja za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 prepovedana napaka: ali je program pridobil žeton, ki ustreza izbranim dovoljenjem?**

Zagotovite, da se vrste dovoljenj, ki jih zahteva ali dodeli, ujemajo z vrsto žetona za dostop, ki ga program pridobi. Morda boste zahtevali in podelili dovoljenja za program, vendar z uporabo pooblaščenih žetonov za pretok kode, namesto žetonov za pretok poverilnic odjemalca, ali zahtevate in odobravanje pooblaščenih dovoljenj, vendar pa uporabite žetone za tokove poverilnic odjemalca namesto pooblaščenih žetonov za pretok kode.

Če želite več informacij o pridobivanju žetonov, glejte:

- [Pridobite dostop v imenu uporabnikov in pooblaščenih dovoljenj](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 avtorizacija kode](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pridobite dostop brez uporabnika (storitev Daemon) in dovoljenja za program](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuth 2,0 Client poverilnice](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 prepovedana napaka: ponastavitev gesla**

Trenutno ni dovoljenj za dovoljenje za uporabo storitev daemon za storitve, ki omogočajo ponastavitev uporabniških gesel. Ti API-ji so podprti le z uporabo interaktivnih prenesenih šifer s pripisanim skrbnikom. Če želite več informacij, glejte [dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference).

**403 Forbidden: ali ima uporabnik dostop do licence?**

Za prenesene tokove kode Microsoft Graph oceni, ali je bila zahteva dovoljena glede na dovoljenja, ki so bila dodeljena programu, in dovoljenja, ki jih je imel prijavljeni uporabnik. Na splošno ta napaka pomeni, da uporabnik ni dovolj privilegiran za izvajanje zahteve **ali** pa uporabnik nima licence za dostop do podatkov. Zahtevi lahko uspešno omogočijo le uporabniki z zahtevanimi dovoljenji ali licencami.

**403 Forbidden: ali ste izbrali ustrezen API vira?**

Storitve API-ja, kot je Microsoft Graph, preverijo, ali se trditev *AUD* (občinstvo) v prejetem žetonu ujema z vrednostjo, ki jo pričakuje zase, in če ne, se zgodi napaka v 403. Pogosta napaka, ki povzroči to napako, poskuša uporabiti žeton, ki je bil kupljen za Azure AD Graph API, Outlook API ali SharePoint/OneDrive API za klicanje Microsoft Graph (ali obratno). Zagotovite, da vir (ali obseg) program pridobi žeton za ujemanje API-ja, ki ga aplikacija kliče.

**400 slaba zahteva ali 403 prepovedana: ali uporabnik upošteva pravilnike za pogojni dostop organizacije (CA)?**

Na podlagi pravilnikov o pogojnem dostopu organizacije (CA) lahko uporabnik, ki dostopa do virov Microsoft Grapha prek vašega programa, ugovarja za dodatne informacije, ki niso na voljo v žetonu za dostop, ki ga je prvotno pridobil. V tem primeru aplikacija prejme **400 z napako *interaction_required*** med pridobitvijo žetona Accessa ali **403 s *insufficient_claims*** napako, ko pokličete Microsoft Graph. V obeh primerih se prikaže sporočilo o napaki, ki vsebuje dodatne informacije, ki jih je mogoče prikazati na pooblaščeni končni točki, da se uporabnik pozove k dodatnim informacijam (na primer preverjanje pristnosti z več dejavniki ali vpis naprave).

Če želite več informacij, povezanih s pogojnim dostopom, glejte:

- [Obravnavanje izzivov s pogojnim dostopom z MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Navodila za razvijalce za pogojni dostop v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice adal) in AZURE ad GRAPH API (zvočni grafikon)_* _

- Z začetkom junija 30th 2020 ne bomo več dodali nobenih novih funkcij v knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL) in Azure AD Graph API (ZVOČNI grafikon). Še naprej bomo zagotavljali tehnično podporo in varnostne posodobitve, vendar ne boste mogli več posredovati posodobitev funkcij.
- Z začetkom junija 30th 2022 bomo zaključili podporo za knjižnice ADAL in ZVOČNI diagram ter ne bodo več zagotavljali tehnične podpore ali varnostnih posodobitev.
    - Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo prejeli nobene tehnične podpore ali varnostnih posodobitev.
    - Programi s pomočjo grafa ZVOČNIh grafikonov po tem času morda ne bodo več prejemali odgovorov v končni točki grafa ZVOČNIh grafikonov.

_ *Knjižnice adal selitev**

Priporočamo, da posodobite [Microsoftovo knjižnico za preverjanje pristnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki ima najnovejše funkcije in varnostne posodobitve. To priporočilo je v kontekstu Microsoft, ki seli svoje aplikacije v MSAL z rokom konca podpore. Cilj selitve aplikacije Microsoft apps na MSAL je zagotoviti, da bodo programi koristili od trenutne varnosti in izboljšav funkcij v MSAL.

- [Preberite pogosta vprašanja o knjižnice ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Preberite več o tem, kako preseliti aplikacije na osnovi na platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, vam priporočamo, da pregledate vse izvorne kode programov in po potrebi dostopate do neodvisnih ponudnikov programske opreme (ISVs) ali ponudnikov programov. Microsoftova podpora vam omogoča tudi seznam vseh programov, ki niso Microsoftovi za knjižnice ADAL, v najemniku.

**Selitev diagrama ZVOČNIh grafikonov**

Za programe, ki uporabljajo ZVOČNI graf, upoštevajte naše napotke za [selitev programov AZURE ad Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Naš kontrolni seznam selitve zagotavlja uvodno mesto](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- V portalu za registracijo aplikacije Azure so prikazani programi, ki uporabljajo ZVOČNI diagram. Priporočamo vam, da pregledate vse izvorne kode programov in po potrebi poiščete vse ponudnike ISVs ali aplikacije. Microsoftova podpora vam lahko zagotovi tudi informacije o uporabi vseh ZVOČNIh grafikonov v najemniku.

 










