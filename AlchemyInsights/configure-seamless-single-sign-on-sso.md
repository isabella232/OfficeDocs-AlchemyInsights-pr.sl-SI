---
title: Konfiguracija nemotene enotne vpise (SSO)
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
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966053"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfiguracija nemotene enotne vpise (SSO)

**Konfiguracija programov**

1. Vrednosti bi morali dobiti pri prodajalcu aplikacij. Vrednosti lahko ročno vnesete ali pa prenesete datoteko metapodatkov, da izvlečete vrednost polj.
2. Številne aplikacije so bile že vnaprej konfigurirane za delo z imenikom Azure AD. Te aplikacije so navedene v galeriji aplikacij, po katere lahko brskate, ko dodate aplikacijo v najemnika Azure AD. V [nizu hitrih zagonov](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) so navodila za ta postopek.
3. Če želite ustvariti program, ki ni galerija, lahko kliknete + Ustvari svoj gumb **»Program«** in poimen uporabljate program.
    - Privzeto je izbrana možnost **Integrirati kateri** koli drug program, ki ga ne najdete v galeriji, kar je prava možnost za aplikacije, ki niso iz galerije.
    - Ko po **vlaganje** imena programa v program pritisnite Ustvari, se ustvari nov program za podjetja, ki ni galerija.
    - Nato se lahko **pomaknete**  do možnosti enotne prijave v razdelku Upravljanje te aplikacije in videli boste lahko različne tehnike za izvedbo programa v vašem okolju.

**Konfiguracija nemotene prijave za določeno aplikacijo**

Za programe v galeriji boste našli podrobna navodila po korakih. Če želite dostopati do korakov, lahko brskate po seznamu vseh vadnic za konfiguracijo aplikacije na vadnicah za konfiguracijo [aplikacije SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfiguracija SSO, ki temelji na SAML**

1. Hitri začetek: Nastavitev enotne prijave [(SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)za program v najemniku Azure Active Directory (Azure AD) s storitvijo SAML.
2. Če želite izvedeti več o možnostih enotne vpise, ki temelji na SAML, glejte Razumevanje enotne vpise, ki [temelji na SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Če želite izvedeti več o zahtevah za preverjanje pristnosti SAML 2.0 in odgovorih, ki jih Azure Active Directory (Azure AD) podpira za enotno Sign-On (SSO), glejte Protokol [SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)za Sign-On single Sign-On .
4. Če želite izvedeti, kako ustvarite in konfigurirate enotno prijavo (SSO) za aplikacijo v storitvi Azure Active Directory (Azure AD) z vmesnikom API za Microsoft Graph, glejte Konfiguracija enotne prijave na osnovi [saml](https://docs.microsoft.com/graph/application-saml-sso-configure-api)za program z vmesnikom API za Microsoft Graph .
5. Če želite izvedeti, kako Azure AD uporablja protokol SAML, glejte [kako Microsoftova platforma za identitete uporablja protokol SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfiguracija žetonov in zahtevkov**

1. [Kako: prilagodite zahtevke, izdane v žetonu SAML za aplikacije za podjetja.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Če želite izvedeti, kako konfigurirate zahtevke z lupino PowerShell, glejte Navodila: prilagajanje zahtev, izpuščenih v žetonih za določen program v najemniku [(predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Če želite izvedeti, kako konfigurirate izbirne zahtevke, glejte [Kako: navedite izbirne zahtevke za program.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Če želite izvedeti, kako uporabiti atribute pripone sheme imenika za pošiljanje uporabniških podatkov programom v zahtevkih po žetonu, glejte Uporaba atributov pripone sheme imenika [v zahtevkih.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Če želite izvedeti, kako konfigurirate življenjske dobe žetonov, glejte Konfiguriranje življenjske dobe žetonov [v Microsoftova platforma za identitete (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfiguracija pravilnikov o življenjskem](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) dobi žetona (predogled) – v tem članku je pogost scenarij skupnega pravilnika, ki vam lahko pomaga uvesti nova pravila za življenjsko dobo žetona. V tem primeru se boste naučili ustvariti pravilnik, ki zahteva, da uporabniki pogosteje preverjajo pristnost v spletni aplikaciji.

**Odpravljanje težav s konfiguracijo SSO**

- Za pogosta vprašanja o nemoteni enotno Azure Active Directory (seamless Sign-On SSO) glejte [Azure Active Directory enotna prijava: pogosta vprašanja.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Če želite informacije o odpravljanju pogostih težav v zvezi Azure Active Directory s nemoteno enotno prijavo (Azure AD) Sign-On enotno prijavo), glejte Odpravljanje težav Azure Active Directory enotno [prijavo.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
