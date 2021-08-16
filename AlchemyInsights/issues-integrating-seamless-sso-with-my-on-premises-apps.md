---
title: Težave z integracijo nemotene storitve SSO z aplikacijami na mestu uporabe
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028308"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Težave z integracijo nemotene storitve SSO z aplikacijami na mestu uporabe

Če želite odpraviti težave z integracijo nemotene storitve SSO z aplikacijami na mestu uporabe, naredite to:

**Priporočeni koraki**

1. Če želite **konfigurirati program na** mestu uporabe za enotno prijavo prek proxyja aplikacije, glejte Shranjevanje gesla za enotno prijavo s [proxyjem aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting). 
1. **Odpravljanje težav s proxyjem** aplikacije: priporočamo, da začnete s pregledovanjem poteka odpravljanja [težav,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)odpravljanje težav s povezovalniki proxy aplikacije, da ugotovite, ali so povezovalniki proxy aplikacije pravilno konfigurirani. Če imate še vedno težave z vzpostavljanjem povezave z aplikacijo, upoštevajte navodila za odpravljanje težav v odpravljanju težav s programčka [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)aplikacije. Težave s [storitvijo CORS lahko prepoznate](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) s spodnjimi orodji za iskanje napak v brskalniku:
    1. Zaženite brskalnik in poiščite spletni program.
    1. Pritisnite **F12,** da pridržite konzolo za iskanje napak.
    1. Poskusite znova pri povzeti transakcijo in preglejte sporočilo konzole. Kršitev cors povzroči napako konzole o izvoru.
    1. Nekaterih težav v zbirki CORS ni mogoče odpraviti, na primer takrat, ko vaša aplikacija preusmeri login.microsoftonline.com za preverjanje pristnosti, žeton za dostop pa poteče. Klic CORS nato ne uspe. Rešitev za ta scenarij je, da podaljšate življenjsko dobo žetona za dostop, da preprečite, da bi potekla med sejo uporabnika. Če želite več informacij o tem, kako to naredite, glejte Konfiguriranje življenjske [dobe žetonov v Microsoftova platforma za identitete](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Priporočeni dokumenti**

- [Konfiguracija enotne prijave v program proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Enotna prijava SAML za programe na mestu uporabe s strežnikom Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Razumevanje in odpravljanje Azure Active Directory težav s strežnikom Application Proxy CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Odpravljanje težav pri konfiguracijah pooblastitev omejitev Kerberos za proxy aplikacije](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)