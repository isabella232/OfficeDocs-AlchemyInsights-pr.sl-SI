---
title: Težave z integracijo brezšivne SSO s programi na mestu uporabe
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868724"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Težave z integracijo brezšivne SSO s programi na mestu uporabe

Če želite odpraviti težave z integracijo brezšivne SSO s programi na mestu uporabe, naredite to:

**Priporočeni koraki**

1. Če želite konfigurirati **program na** mestu uporabe za **enotno prijavo prek proxya programa**, si oglejte [Iskanje gesla za enotno prijavo s proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Odpravljanje težav s proxyjem aplikacije**: priporočamo, da začnete s pregledovanjem toka odpravljanja težav, [težav s povezovalnikom strežnika debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), če želite ugotoviti, ali so povezovalniki proxy programov pravilno konfigurirani. Če imate še vedno težave z vzpostavljanjem povezave z aplikacijo, upoštevajte navodila za odpravljanje težav v aplikaciji [aplikacije proxy programa debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Težave z [CORS lahko prepoznate](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) tako, da uporabite ta orodja za iskanje napak brskalnika:
    1. Zaženite brskalnik in prebrskajte do spletnega programa.
    1. Pritisnite **F12** , da prikažete konzolo Debug.
    1. Poskusite znova ustvariti transakcijo in preglejte konzolno sporočilo. Zaradi kršitve CORS se prikaže konzolna napaka o poreklu.
    1. Nekaterih težav z CORS ni mogoče razrešiti, na primer, ko se aplikacija preusmeri v login.microsoftonline.com za preverjanje pristnosti, in je žeton za dostop potekel. Klic CORS nato spodleti. Rešitev tega scenarija je, da podaljšate življenjsko dobo Accessovega žetona, da preprečite, da bi poteklo med sejo uporabnika. Če želite več informacij o tem, kako to naredite, glejte [Doživljenjska doba žetonov v Microsoftovi platformi za identiteto](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Priporočeni dokumenti**

- [Kako konfigurirati enotno prijavo v aplikacijo proxy programa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [SAML enotne prijave za aplikacije na mestu uporabe z proxyjem programa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Razumevanje in reševanje težav z proxyjem storitve Azure Active Directory CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Odpravljanje težav s omejena konfiguracija dodeljevanja Kerberos za proxy programa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)