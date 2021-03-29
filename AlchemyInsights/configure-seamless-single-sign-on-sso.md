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
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402283"
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

1. Hitri začetek: nastavitev enotne prijave [(SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)za SAML za aplikacijo v najemniku imenika Azure Active Directory (Azure AD).
2. Če želite izvedeti več o možnostih enotne vpise, ki temelji na SAML, glejte Razumevanje enotne vpise, ki [temelji na SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Če želite izvedeti več o zahtevah za preverjanje pristnosti SAML 2.0 in odgovorih, ki jih Azure Active Directory (Azure AD) podpira za enotno Sign-On (SSO), glejte Protokol SAML za Sign-On enotno [uporabo.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Če želite izvedeti, kako ustvarite in konfigurirate enotno prijavo (SSO) za aplikacijo v imeniku Azure Active Directory (Azure AD) z api-jem Microsoft Graph API, glejte Konfiguracija enotne prijave za program, ki temelji na [SAML,](https://docs.microsoft.com/graph/application-saml-sso-configure-api)z vmesnikom API za Microsoft Graph.
5. Če želite izvedeti, kako Azure AD uporablja protokol SAML, glejte [Kako Microsoftova platforma identitete uporablja protokol SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfiguracija žetonov in zahtevkov**

1. [Kako: prilagodite zahtevke, izdane v žetonu SAML za aplikacije za podjetja.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Če želite izvedeti, kako konfigurirate zahtevke z lupino PowerShell, glejte Navodila: prilagajanje zahtev, izpuščenih v žetonih za določen program v najemniku [(predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Če želite izvedeti, kako konfigurirate izbirne zahtevke, glejte [Kako: navedite izbirne zahtevke za program.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Če želite izvedeti, kako uporabiti atribute pripone sheme imenika za pošiljanje uporabniških podatkov programom v zahtevkih po žetonu, glejte Uporaba atributov pripone sheme imenika [v zahtevkih.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Če želite izvedeti, kako konfigurirate življenjske dobe žetonov, glejte Življenjske dobe žetonov, ki jih je mogoče konfigurirati v Microsoftovi [platformi za identitete (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfiguracija pravilnikov o življenjskem](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) dobi žetona (predogled) – v tem članku je pogost scenarij skupnega pravilnika, ki vam lahko pomaga uvesti nova pravila za življenjsko dobo žetona. V tem primeru se boste naučili ustvariti pravilnik, ki zahteva, da uporabniki pogosteje preverjajo pristnost v spletni aplikaciji.

**Odpravljanje težav s konfiguracijo SSO**

- Za pogosta vprašanja o nemoteni enotno prijavo v imenik Azure Active Directory (nemotena enotna prijava) Sign-On [Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)pogosta vprašanja.
- Če želite informacije o odpravljanju pogostih težav glede nemotene enotne enotne Sign-On imenika Azure Active Directory (Azure AD), glejte Odpravljanje težav s nemoteno enotno prijavo v [imenik Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)
