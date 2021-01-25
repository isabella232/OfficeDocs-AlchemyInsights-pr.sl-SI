---
title: Težave s povezavami in spletnimi naslovi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974754"
---
# <a name="issues-with-links-and-urls"></a>Težave s povezavami in spletnimi naslovi

Preusmerjanje URI/URL-ji odgovorov (Oba izraza sta medsebojno izmenljiva) so URL-ji, ki jih uporablja Microsoftova identitetna platforma za vrnitev žetonov, ki jih zahteva program. Če želite več informacij o teh URL-jih, si oglejte te članke:

- [Tokovi preverjanja pristnosti in scenariji uporabe](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacije o preusmeritvi URI-jev na strani za **registracijo aplikacije** za vsak scenarij.
- [Preusmeritev in omejitve URL-ja/odgovorov](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ne vem, kako naj registriram ustrezen URI/odgovori URL za moj program**

Ko se vpišete z aplikacijo, ki jo razvijate, če se v pogovornem oknu za vpis prikaže **AADSTS50011: URL odgovora, ki je naveden v zahtevi, se ne ujema z URL- <your app ID> ji odgovora, konfiguriranimi za aplikacijo**, morate dodati v registracijo aplikacije, preusmeritveni uri, ki ga je vaša koda uporabila v zahtevi za žeton za Microsoftovo platformo Identity.

Če želite dodati URL odgovora, pojdite na zavihek **preverjanje pristnosti** na strani za **registracijo aplikacije** v portalu Azure in dodajte vnos v razdelek» **preusmeritev URIs** «. Preusmeritveni uri-ji so vneseni (splet ali prenosni/namizni). Vrednost, ki jo morate vnesti, je odvisna od vrste programa, ki ga gradite, kot je opisano spodaj:

- Za aplikacije z eno stranjo in spletne aplikacije je URL odgovora URL v vaši aplikaciji. Glejte [registracija aplikacije na eni strani](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ali registracija aplikacije [Web App s portalom Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Za namizne aplikacije je vrednost, ki jo morate izbrati, odvisna od:
    - platforma (MacOS se razlikuje od sistema Windows ali Linux)
    - način pridobitve žetona (interaktivno s tokom kode naprave z integriranim preverjanjem pristnosti sistema Windows [IWA] ali z uporabniškim imenom/geslom).
    Če želite več informacij, glejte [namizne aplikacije – registracija programov – preusmeritev URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Za prenosne aplikacije je URI za preusmeritev odvisen od:
    - platforma (iOS/Android/UWP)
    - informacije, ki se uporabljajo za izgradnjo aplikacije, kot je ID za snop v sistemu iOS, in razpršilno ime paketa ter razprševanje podpisa v sistemu Android, ki vam bo v pomoč pri registraciji aplikacije Azure portal. Če želite več informacij, glejte [Konfiguracija platforme in preusmeritev URI-jev](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Spletni vmesniki API in nekateri tihi načini pridobivanja žetonov (IWA in uporabniško ime/geslo) ne potrebujete URI za preusmeritev.

**Uvedl sem spletni program in ko sem testiral uveden program, dobim sporočilo o neujemanju URL-ja odgovora.**

Dodajte preusmeritvene uri-je za vsa mesta, na katerih uvajate spletni program. Če želite več informacij, glejte [registriranje aplikacije Web App s portalom Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Dodajte preusmeritveni URI za mesto takoj, ko ste uvedli program na tem mestu.

**Ne morem se registrirati dovolj URL-jev za odgovore**

Vi ste VMESNa odprava in imate enega ali več preusmeritvenih uri za vsako vašo stranko. Želite preseliti iz knjižnice ADAL/Azure AD v 1.0 na MSAL/Microsoft Identity platform in ste zadeli [največje število preusmeritev URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Če želite odpraviti to težavo, [dodajte preusmeritvene uri-je za upravnike storitev](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , ki ustrezajo posameznim strankam.
