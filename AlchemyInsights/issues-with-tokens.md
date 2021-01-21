---
title: Težave z žetoni
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
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917033"
---
# <a name="issues-with-tokens"></a>Težave z žetoni

Če želite upravljati težave, povezane z žetoni, lahko izvedete te korake:

1. Določite lahko življenjsko dobo Accessovega, ID-ja ali SAML žetona, ki ga je izdala Microsoftova platforma za identiteto. Življenjske dobe žetonov lahko nastavite za vse programe v organizaciji, za program multi-najemnika (multi-Organization) ali za določenega glavnega ponudnika v organizaciji. Če želite več informacij, glejte [prilagodljiva življenjska doba žetonov v Microsoftovi identiteti platforme (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Žetoni za Access omogočajo odjemalcem, da varno pokličejo zaščitene spletne vmesnike API in jih uporabljajo spletni API-ji za izvajanje preverjanja pristnosti in avtorizacije. Kot na specifikaciji OAuth so žetoni za dostop neprozorni nizi brez nabora oblik – nekateri ponudniki identitete (NRO) uporabljajo GUID-i, drugi pa uporabljajo šifrirane blobe. Platforma Microsoft Identity uporablja različne oblike Accessovega žetona, odvisno od konfiguracije API-ja, ki sprejme žeton. Če želite izvedeti, kako lahko API preveri veljavnost in uporabite terjatve znotraj žetona za dostop, si oglejte [žetoni za dostop do Microsoftovega](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)uporabniškega vmesnika.
3. Microsoftova knjižnica za preverjanje pristnosti (MSAL) podpira več tokov preverjanja pristnosti za uporabo v različnih scenarijih programov. Če želite več informacij, glejte [tokovi preverjanja pristnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Odobritev kode za avtorizacijo OAuth 2,0 lahko uporabite v aplikacijah, ki so nameščene v napravi, da pridobijo dostop do zaščitenih virov, kot so spletni vmesniki API. Če uporabljate Microsoftovo 2,0 platformo Identity, lahko v mobilne in namizne aplikacije dodate dostop do vpisov in API-ja. Če želite, da program neposredno upošteva protokol v aplikaciji, uporabite kateri koli jezik, si oglejte [platformo Microsoft Identity in koda za avtorizacijo OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) .
5. OpenID povezava (OIDC) je protokol za preverjanje pristnosti, ki je zgrajen na spletnem mestu OAuth 2,0, ki ga lahko uporabite za varno vpis uporabnika v aplikacijo. Ko uporabite funkcijo končne točke izvajanja storitve OpenID za Microsoft Identity, lahko v programe dodate dostop za vpis in API. [Microsoft Identity platform in protokol za povezavo OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) prikazuje, kako to naredite neodvisno od jezika in kako pošiljati in PREJEMATI sporočila http brez uporabe katerega koli Microsoftovega knjižnic z odprtim izvorom.
    - Končna točka UserInfo je del standarda OIDC, ki je zasnovan tako, da vrne terjatve do uporabnika, ki je bil preverjen. Če želite več informacij, glejte [končna točka UserInfo na platformi Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Klicanje spletnega API-ja v spletnem programu z uporabo storitve AZURE ad in OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) Sample prikazuje, kako zgraditi spletni program MVC, ki uporablja Azure ad za vpis s protokolom za povezavo OpenID, in nato pokličete spletni vmesnik API v skladu s prijavljeno identiteto uporabnika z žetoni, pridobljenimi prek storitve OAuth 2,0. Ta vzorec uporablja poverilnice OpenID Connect ASP .net OWIN vmesni in knjižnice ADAL .net.
6. [Konfigurirajte aplikacijo za razkrivanje spletnega API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -v tej hitri različici, registrirate spletni API s platformo Microsoft Identity in jo izpostavite v odjemalske aplikacije tako, da dodate vzorčni obseg. Ko registrirate spletni vmesnik API in ga izpostavite prek obsegov, lahko na podlagi dovoljenj omogočite dostop do svojih virov za pooblaščene uporabnike in odjemalske aplikacije, ki dostopajo do vašega API-ja.
7. V storitvi Azure Active Directory B2C (Azure AD B2C) so poverilnice, ki jih ima lastnik za gesla (ROPC), tok za preverjanje pristnosti, ki je standard OAuth. V tem toku program, imenovan tudi» sklicujoč se «, izmenjuje veljavne poverilnice za žetone. Poverilnice vključujejo ID uporabnika in geslo. Vrnjeni žetoni so žeton za ID, žeton za dostop in žeton za osveževanje. Če želite več informacij, glejte [nastavitev sistema poverilnic za gesla lastnika vira v storitvi Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

