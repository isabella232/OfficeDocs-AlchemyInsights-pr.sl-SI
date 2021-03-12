---
title: Težave s povezavami in URL-ji
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707898"
---
# <a name="issues-with-links-and-urls"></a>Težave s povezavami in URL-ji

URL-ji preusmeritve/odgovora (oba izraza sta izmenljiva) so URL-ji, ki jih Microsoftova platforma za identitete uporablja za vrnitev žetonov, zahtevanih s programom. Če želite informacije o teh URL-jih, glejte te članke:

- [Pretoki preverjanja pristnosti in scenariji uporabe](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacije o URL-jih preusmeritve na strani za registracijo **aplikacije** posameznega scenarija.
- [Omejitve URL-ja preusmeritve/odgovora](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Ne vem, kako registrirati pravi URI preusmeritve/URL za odgovor za svoj program**

Če se ob vpisu z aplikacijo, ki jo razvijate, prikaže pogovorno okno za vpis **AADSTS50011: URL za odgovor, ki je naveden v zahtevi, se ne ujema z URL-ji za odgovore, konfiguriranimi za aplikacijo <your app ID>**, boste morali dodati k registraciji programa, URI za preusmerjanje, ki ga je koda, uporabljena v zahtevi žetona, za Microsoftovo platformo za identitete.

Če želite dodati URL za odgovor, pojdite na zavihek **Authentication** na strani za registracijo aplikacije **v portalu Azure** dodajte vnos v razdelek **Redirect URL** (Preusmeri URL-je). Vrednost, ki jo morate vnesti, je odvisna od vrste programa, ki ga gradite, kot je opisano spodaj:

- Pri programih z eno stranjo in spletnih aplikacijah je URL odgovora URL v vaši aplikaciji. Oglejte [Registracija eno stran programa](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ali [Registracija spletnega programa s portalom Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Za namizne programe je vrednost, ki jo morate izbrati, odvisna od:
    - platforma (MacOS se razlikuje od sistema Windows ali Linux)
    - način pridobivanja žetona (interaktivno s tokom kode naprave, z integriranim preverjanjem pristnosti sistema Windows [IWA] ali z uporabniškim imenom/geslom).
    Če želite več podrobnosti, glejte [namizne aplikacije – registracija aplikacije – Preusmerjanje URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Za mobilne aplikacije je URI preusmeritve odvisen od tega:
    - platforma (iOS/Android/UWP)
    - informacije, uporabljene za ustvarjanje aplikacije, kot je ID svežnja v sistemu iOS, ter ime paketa in razdvoji podpis v sistemu Android Registracija aplikacije v portalu Azure vam bo pomagala. Podrobnosti najdete v [konfiguracije platforme in preusmeritve URL-jev](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Spletni API-ji in nekateri tihi načini pridobivanja žetonov (IWA in uporabniško ime/geslo) ne zahtevajo URI-ja preusmeritve.

**Uvedel sem spletni program in ko preskusim uvedeno aplikacijo, se prikaže sporočilo o ne spletnem naslovu za odgovor**

Dodajte URL-je preusmeritve za vsa mesta, na katerih uvajate spletni program. Če želite več informacij, glejte [Registracija spletnega programa s portalom Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> URI preusmeritve za mesto dodajte takoj, ko uvedete program na tem mestu.

**Ne morem registrirati dovolj URL-jev za odgovor**

Ste ISV in imate enega ali več URL-jev za preusmerjanje za vsako stranko. Iz storitve ADAL/Azure AD v1.0 želite preseliti v platformo za identitete MSAL/Microsoft in pri tem morate [največje dovoljeno število URL-jev za preusmeritev](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). To težavo odpravite tako, [dodate URL-je preusmeritve k glavnim](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), ki ustrezajo vsaki posamezni stranki.
