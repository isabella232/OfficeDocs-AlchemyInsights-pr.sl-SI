---
title: Odpravljanje težav s nemoteno enotno prijavo na osnovi OIDC
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
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105794"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Odpravljanje težav s nemoteno enotno prijavo na osnovi OIDC

- Če želite izvedeti, kako dodate aplikacijo, ki temelji na storitvi OIDC, v najemnika Azure, glejte Vodnik za hitri začetek: Nastavitev enotne prijave [(SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)za aplikacijo v najemniku storitve Azure Active Directory (Azure AD).
- Če želite več podrobnosti o aplikacijah, ki uporabljajo standard OpenID Povezovalnik standard za enotno prijavo, glejte Razumevanje enotne vpise na osnovi [OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Za informacije, če se odločite za pisanje kode tako, da pošljete in obravnavate zahteve HTTP ali uporabite odprtokodno knjižnico drugega lokacije, namesto da bi uporabili eno od naših odprtokodnih knjižnic, glejte [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)in OpenID Povezovalnik protocols on the Microsoftova platforma za identitete .

**Protokoli**

1. Microsoftova platforma za identitete in [implicitni](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) grant flow – definiranje značilnosti implicitne dodelitve je, da se žetoni (žetoni ID-ja ali žetoni za dostop) vrnejo neposredno iz končne točke /authorize namesto končne točke /token. To se pogosto uporablja kot del poteka avtorizacijske kode, v tako imenovanem **»hibridni** tok« – pridobivanje žetona ID-ja na zahtevi /authorize skupaj s avtorizmsko kodo . V tem članku je opisano, kako program neposredno prek protokola v aplikaciji zahtevate žetone imenika Azure AD.
2. Microsoftova platforma za identitete in postopek avtorizacije [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – podelitev avtorizatne kode OAuth 2.0 lahko uporabite v programih, nameščenih v napravi, za pridobitev dostopa do zaščitenih virov, kot so spletni API-ji. Z Microsoftova platforma za identitete OAuth 2.0 lahko dodate vpis in dostop do API-ja v **mobilnih in namiznih aplikacijah.** V tem članku je opisano, kako program neposredno uporabite v programu v katerem koli jeziku.
3. Microsoftova platforma za identitete protokol [Povezovalnik OpenID –](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) če uporabljate izvajanje Microsoftova platforma za identitete OpenID Povezovalnik, lahko dodate vpis in dostop do API-ja v aplikacije. V tem članku je opisano, kako to naredite neodvisno od jezika, opisano pa je tudi, kako pošiljati in prejemati sporočila HTTP brez **Microsoftovih odprtokodnih knjižnic.**
4. Microsoftova platforma za identitete in tok poverilnic [odjemalca OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – za dostop do virov, ki gostujejo v spletu, z identiteto programa lahko uporabite poverilnice odjemalca OAuth 2.0, določene v RFC 6749, včasih imenovanem **two-legged OAuth.** Ta vrsta dodelitve se pogosto uporablja za interakcije med strežniki, ki se morajo izvajati v ozadju, brez takojšnjega sodelovanja z uporabnikom. Te vrste aplikacij pogosto imenujemo tudi **daemone ali** **računi storitev.** V tem članku je opisano, kako program neposredno programi v programu.
