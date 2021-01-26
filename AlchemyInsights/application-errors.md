---
title: Napake aplikacije
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984658"
---
# <a name="application-errors"></a>Napake aplikacije

Iščete informacije o **AADSTS kodah napak** , ki so bile vrnjene v storitvi za varnost žetona Azure Active Directory ("Azure ad)" (STS)? Preberite [kode napak za preverjanje pristnosti in avtorizacije AZURE ad](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , da poiščete opise napak AADSTS, popravke in nekatere predlagane rešitve.

Napake pri avtorizaciji so lahko rezultat več različnih težav, od katerih večina ustvari napako 401 ali 403. To lahko na primer privede do napak pri avtorizaciji:

- Nepravilni [tokovi za pridobitev žetona](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Slabo konfigurirani [obsegi dovoljenj](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Pomanjkanje [soglasja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Če želite odpraviti pogoste napake avtorizacije, preskusite spodaj navedene korake, ki se najbolj ujemajo z napako, ki jo prejemate. Uporabite lahko več kot eno.

**nepooblaščena Napaka 401: ali je žeton veljaven?**

Zagotovite, da vaš program predstavlja veljaven žeton za dostop v Microsoft Graph kot del zahteve. Ta napaka pogosto pomeni, da žeton za dostop morda manjka v glavi zahteve za preverjanje pristnosti HTTP ali da je žeton neveljaven ali pa je potekel. Toplo priporočamo, da uporabite [Microsoftovo knjižnico za preverjanje pristnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) za pridobitev žetona za dostop. Poleg tega lahko pride do te napake, če poskušate za dostop do API-ja, ki podpira le službene ali šolske račune (organizacijske račune), dodeliti žeton za pooblaščen dostop, ki je dodeljen osebnim Microsoftovim računom.

**403 prepovedana napaka: ali ste izbrali pravi nabor dovoljenj?**

Preverite, ali ste zahtevali pravilen nabor dovoljenj, ki temeljijo na aplikaciji Microsoft Graph API aplikacije. Priporočena najmanj privilegirana dovoljenja so na voljo v vseh temah referenčne metode za Microsoft Graph API. Poleg tega morajo ta dovoljenja odobriti aplikacija uporabnik ali skrbnik. Dodeljevanje dovoljenj se običajno zgodi prek strani s privolitvijo ali z uporabo rezila za registracijo aplikacije Azure portal. Iz rezila z **nastavitvami** za aplikacijo kliknite **zahtevana dovoljenja** in nato še **dodeli dovoljenja**.

- [Dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Razumevanje dovoljenj in soglasja za Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 prepovedana napaka: ali je program pridobil žeton, ki ustreza izbranim dovoljenjem?**

Prepričajte se, da je vrsta dovoljenj, ki jih zahteva ali dodeli, enaka vrsti žetona za dostop, ki ga program pridobi. Morda boste zahtevali in podelili dovoljenja za program, vendar z uporabo pooblaščenih žetonov za pretok kode, namesto žetonov za pretok poverilnic odjemalca, ali zahtevate in odobravanje pooblaščenih dovoljenj, vendar pa uporabite žetone za tokove poverilnic odjemalca namesto pooblaščenih žetonov za pretok kode.

- [Pridobite dostop v imenu uporabnikov in pooblaščenih dovoljenj](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 avtorizacija kode](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Pridobite dostop brez uporabnika (storitev Daemon) in dovoljenja za program](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuth 2,0 Client poverilnice](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 prepovedana napaka: ponastavitev gesla**

Trenutno ni dovoljenj za dovoljenje za uporabo storitev daemon za storitve, ki omogočajo ponastavitev uporabniških gesel. Ti API-ji so podprti le z uporabo interaktivnih prenesenih šifer s pripisanim skrbnikom.

- [Dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference)

**403 Forbidden: ali ima uporabnik dostop do licence?**

Za prenesene tokove kode se Microsoft Graph ovrednoti, če je zahtevo dovoljeno glede na dovoljenja, ki so dodeljena programu, in dovoljenja, ki jih je imel prijavljeni uporabnik. Na splošno ta napaka pomeni, da uporabnik ni dovolj privilegiran za izvajanje zahteve ali pa uporabnik nima licence za dostop do podatkov. Zahtevi lahko uspešno omogočijo le uporabniki z zahtevanimi dovoljenji ali licencami.

**403 Forbidden: ali ste izbrali ustrezen API vira?**

Storitve API, kot je Microsoft Graph, preverijo, ali se trditev AUD (občinstvo) v prejetem žetonu ujema z vrednostjo, ki jo pričakuje zase, in če je ne, povzroči napako v 403, ki je prepovedana. Pogosta napaka, ki povzroči to napako, poskuša uporabiti žeton, ki je bil kupljen za Azure AD Graph API, Outlook API ali SharePoint/OneDrive API za klicanje Microsoft Graph (ali obratno). Zagotovite, da vir (ali obseg) program pridobi žeton za ujemanje API-ja, ki ga aplikacija kliče.

**400 slaba zahteva ali 403 prepovedana: ali uporabnik upošteva pravilnike za pogojni dostop organizacije (CA)?**

Na podlagi pravilnikov CA organizacije se lahko uporabnik, ki dostopa do virov Microsoft Grapha prek vašega programa, pozove k dodatnim podatkom, ki niso na voljo v žetonu za dostop, ki ga je prvotno pridobil. V tem primeru aplikacija prejme 400 z napako *interaction_required* med pridobitvijo žetona Accessa ali 403 s *insufficient_claims* napako, ko pokličete Microsoft Graph. V obeh primerih je odgovor na sporočilo o napaki prikazan v dodatnih informacijah, ki jih je mogoče predstaviti na končni točki pooblastitev, da bi izzvali uporabnika za dodatne informacije (na primer preverjanje pristnosti z več dejavniki ali vpis naprave).

- [Obravnavanje izzivov s pogojnim dostopom z MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Navodila za razvijalce za pogojni dostop v storitvi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
