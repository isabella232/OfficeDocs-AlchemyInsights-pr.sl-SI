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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084362"
---
# <a name="sso-connection-issues"></a>Težave s povezavo SSO

1. Upoštevajte [vodnik za hitri začetek: konfigurirajte lastnosti vodnika](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) za program za konfiguracijo aplikacije.
2. Upoštevajte ustrezna navodila spodaj, odvisno [od](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) aplikacije in možnosti enotne prijave, ki ste jo izbrali:
    - Če želite **konfigurirati** aplikacijo na mestu uporabe za enotno prijavo na osnovi **SAML,** glejte Enotna prijava SAML za aplikacije na mestu uporabe s strežnikom [Application Proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Če želite **konfigurirati program v** oblaku za enotno prijavo na osnovi **gesla,** glejte [Konfiguracija enotne prijave gesla.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Če želite **konfigurirati program na** mestu uporabe za enotno prijavo prek proxyja aplikacije, glejte Shranjevanje gesla za enotno prijavo s [proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting). 
3. **Odpravljanje težav s proxyjem** aplikacije: priporočamo, [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)da začnete s pregledovanjem poteka odpravljanja težav, odpravljanje težav s povezovalniki proxy aplikacije, da ugotovite, ali so povezovalniki proxy aplikacije pravilno konfigurirani. Če imate še vedno težave z vzpostavljanjem povezave s aplikacijo, upoštevajte navodila za odpravljanje težav v odpravljanju [težav z aplikacijo Proxy aplikacije.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Težave s [storitvijo CORS lahko prepoznate](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) z orodji za iskanje napak v brskalniku:
    - Zaženite brskalnik in poiščite spletni program.
    - Pritisnite **F12,** da pridržite konzolo za iskanje napak.
    - Poskusite znova pri povzeti transakcijo in preglejte sporočilo konzole. Kršitev cors povzroči napako konzole o izvoru.
    - Nekaterih težav v zbirki CORS ni mogoče odpraviti, na primer takrat, ko vaša aplikacija preusmeri login.microsoft.com za preverjanje pristnosti, žeton za dostop pa poteče. Klic CORS nato ne uspe. Rešitev za ta scenarij je, da podaljšate življenjsko dobo žetona za dostop, da preprečite, da bi potekla med sejo uporabnika. Če želite več informacij o tem, kako to naredite, glejte Konfiguriranje življenjske [dobe žetonov v Microsoftova platforma za identitete](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. Odpravljanje težav z enotno prijavo, ki temelji na **SAML:** priporočamo, da preverite težave pri vpisu v konfigurirane aplikacije za enotno prijavo, ki uporabljajo [SAML, da](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)najdete rešitve za težave, na katere boste najverjetneje naleteli.
5. **Odpravljanje težav z enotno** prijavo na osnovi gesla: priporočamo, da preverite odpravljanje težav z enotno prijavo na osnovi gesla v imeniku [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)da najdete rešitve za težave, na katere boste najverjetneje naleteli.
6. Če želite več informacij o težavah s povezavo med uporabo omrežja VPN, glejte Uporaba enotne enotne Wi-Fi [(SSO) prek omrežja VPN](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)in Wi-Fi povezave.
