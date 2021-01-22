---
title: Težave s povezavo SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935160"
---
# <a name="sso-connection-issues"></a>Težave s povezavo SSO

1. Če želite konfigurirati aplikacijo, uporabite navodila [za hitri začetek: Konfiguracija lastnosti za](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vodnika za aplikacijo.
2. Odvisno od možnosti aplikacija in [enotne prijave](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) , ki ste jo izbrali, upoštevajte spodnja navodila:
    - Če želite konfigurirati **program na** mestu uporabe za **enotno prijavo v SAML**, glejte [SAML z enim samim vpisom za aplikacije na mestu uporabe z proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Če želite konfigurirati **aplikacijo v oblaku** za **enotno prijavo na osnovi gesla**, glejte  [Konfiguracija gesla za enotno prijavo](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Če želite konfigurirati **program na** mestu uporabe za **enotno prijavo prek proxya programa**, si oglejte [Iskanje gesla za enotno prijavo s proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Odpravljanje težav s proxyjem aplikacije**: Priporočamo vam, da začnete s pregledovanjem toka odpravljanja težav, [težav s povezovalnikom strežnika debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), če želite ugotoviti, ali so povezovalniki proxy programov pravilno konfigurirani. Če imate še vedno težave z vzpostavljanjem povezave z aplikacijo, v razdelku težave z aplikacijo [Proxy programa debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)uporabite potek odpravljanja težav. Težave z [CORS lahko prepoznate](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) tako, da uporabite orodja za iskanje napak v brskalniku:
    - Zaženite brskalnik in prebrskajte do spletnega programa.
    - Pritisnite **F12** , da prikažete konzolo Debug.
    - Poskusite znova ustvariti transakcijo in preglejte konzolno sporočilo. Zaradi kršitve CORS se prikaže konzolna napaka o poreklu.
    - Nekaterih težav z CORS ni mogoče razrešiti, na primer, ko se aplikacija preusmeri v login.microsoft.com za preverjanje pristnosti, in je žeton za dostop potekel. Klic CORS nato spodleti. Rešitev tega scenarija je, da podaljšate življenjsko dobo Accessovega žetona, da preprečite, da bi poteklo med sejo uporabnika. Če želite več informacij o tem, kako to naredite, glejte [Doživljenjska doba žetonov v Microsoftovi platformi za identiteto](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Odpravljanje težav z enotno prijavo v SAML**: priporočamo, da preverite težave z vpisom [v SAML, ki temeljijo na konfiguriranih programih enotne prijave](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), da poiščete rešitve za težave, ki jih najpogosteje srečujete.
5. **Odpravljanje težav z enotno prijavo z geslom**: Priporočamo vam, da v storitvi Azure ad poiščete rešitev za [Odpravljanje težav z geslom](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), ki jih boste najverjetneje srečali.
6. Če želite težave s povezavo med uporabo VPN, glejte [Uporaba enotne prijave (SSO) prek VPN in Wi-Fi povezav](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
