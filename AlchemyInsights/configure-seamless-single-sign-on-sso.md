---
title: Konfiguracija nemotene enotne prijave (SSO)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004344"
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841672"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfiguracija nemotene enotne prijave (SSO)

**Konfiguracija programov**

1. Vrednosti iz prodajalca aplikacije bi morali dobiti. Če želite ekstrahirati vrednost polj, lahko ročno vnesete vrednosti ali prenesete datoteko s metapodatki.
2. Številne aplikacije so že konfigurirane za delo s storitvijo Azure AD. Ti programi so navedeni v galeriji programov, ki jih lahko brskate, ko dodate aplikacijo v najemnika storitve Azure AD. [Serija hitrih](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) prehajanja vas popelje skozi postopek.
3. Če želite ustvariti aplikacijo, ki ni v galeriji, lahko kliknete **+ Ustvari svoj** gumb za aplikacijo in poimenujete aplikacijo.
    - Privzeto bo izbrala **vključitev katerega koli drugega programa, ki ga ne najdete v galeriji** , ki je pravilna možnost za aplikacije, ki niso galerije.
    - Ko naletite na ustvarjanje, potem ko ste **ustvarili** ime za aplikacijo, bo ustvarilo novo podjetje, ki ne uporablja galerije.
    - Nato se lahko pomaknete na **enotno prijavo** v razdelku **upravljanje** tega programa in videli boste različne tehnike za njegovo izvajanje v okolju.

**Konfiguracija brezšivne SSO za določen program**

Za programe v galeriji boste našli podrobna navodila po korakih. Če želite dostopati do korakov, si lahko ogledate seznam vseh vadnic za konfiguracijo programov na [vadnicah za konfiguracijo aplikacije SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Konfiguracija SSO, ki temelji na SAML**

1. [Hitri zagon: nastavitev enotne prijave na osnovi SAML (SSO) za aplikacijo v najemniku storitve Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Če želite izvedeti več o možnosti SAML, ki temelji na enotni prijavi, glejte [razumevanje enotne prijave na SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Če želite izvedeti več o zahtevah za preverjanje pristnosti v SAML 2,0 in odgovorih, ki jih Azure Active Directory (Azure AD) podpira za eno Sign-On (SSO), glejte [single Sign-On SAML Protocol](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Če želite izvedeti, kako ustvarite in konfigurirate enotno prijavo v SAML (SSO) za vašo aplikacijo v storitvi Azure Active Directory (Azure AD), ki uporablja Microsoft Graph API, glejte [Konfiguracija SAML z aplikacijo Microsoft GRAPH API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Če želite izvedeti, kako Azure AD uporablja protokol SAML, si oglejte, [Kako Microsoftova identitetna platforma uporablja protokol SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfiguracija žetonov in terjatev**

1. [Kako: prilagajanje terjatev, ki so bile izdane v SAML žeton za podjetja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Če želite izvedeti, kako konfigurirate terjatve z uporabo lupine PowerShell, glejte [Kako: prilagajanje terjatev, ki jih oddajajo žetoni za določen program v najemniku (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Če želite izvedeti, kako konfigurirati izbirne zahtevke, [si oglejte navodila za: Omogočanje izbirnih zahtevkov za vašo aplikacijo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Če želite izvedeti, kako uporabiti atribute razširitve sheme imenika za pošiljanje uporabniških podatkov aplikacijam v zahtevkih žetonov, glejte [Uporaba atributov pripone imenika v zahtevkih](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Če želite izvedeti, kako konfigurirate življenjska doba žetonov, glejte konfiguracija [življenj žetona na Microsoftovi identiteti (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfiguracija veljavnostnih pravilnikov žetona (predogled)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – v tem članku se sprehajamo po skupnem scenariju pravilnika, ki vam lahko pomaga naložiti nova pravila za življenjsko dobo žetonov. V tem primeru se boste naučili ustvariti pravilnik, ki zahteva, da uporabniki preverjajo pristnost v spletnem programu.

**Odpravljanje težav s konfiguracijo SSO**

- Če želite najpogostejša vprašanja o storitvi Azure Active Directory brezšivne Single Sign-On (brezšivne SSO), si oglejte [nemotena Enotna prijava imenika Azure Active Directory: pogosta vprašanja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Če želite informacije o odpravljanju težav s pogostimi težavami v zvezi z imenikom Azure Active Directory (Azure AD) brezšivne Single Sign-On (brezšivne SSO), glejte [Odpravljanje težav z enotno prijavo storitve Azure Active](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
