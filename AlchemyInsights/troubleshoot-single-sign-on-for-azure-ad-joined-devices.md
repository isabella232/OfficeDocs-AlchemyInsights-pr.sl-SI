---
title: Odpravljanje težav z enim samim vpisom za naprave v storitvi Azure AD
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037333"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Odpravljanje težav z enim samim vpisom za naprave v storitvi Azure AD

Če imate okolje Active Directory (AD) na mestu uporabe in se želite pridružiti računalnikom, povezanim z domeno OGLASa, v storitvi Azure AD, lahko to dosežete tako, da izvedete hibridno pridružitev za oglase. [Kako: načrtovati vaš hibridni postopek združevanja v storitvi Hybrid Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) vam ponuja povezane korake za izvajanje hibridnega združevanja oglasov v okolju.

Če želite več informacij, glejte [Konfiguracija naprav v storitvi AZURE ad JOIN za Single-Sign na mestu uporabe v storitvi Windows hello za podjetja](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).

**Težave primarnega osveževanja (PRT)**

Primarni žeton za osveževanje (PRT) je ključni artefakt za preverjanje pristnosti storitve Azure AD v sistemih Windows 10, Windows Server 2016 in novejših različicah, iOS in naprave s sistemom Android. Gre za spletni žeton JSON (JWT), ki je posebej izdan za posrednike za žetone Microsoft First Party, da omogoči enotno prijavo (SSO) med programi, ki so uporabljeni v teh napravah. Če želite več informacij o tem, kako je PRT izdan, uporabljen in zaščiten v napravah s sistemom Windows 10, glejte [Kaj je primarni žeton za osveževanje?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: da in AzureADPrt: da**

V teh poljih je navedeno, ali se je uporabnik uspešno potrdil na Azure AD, ko se je prijavljal v napravo. Če **vrednosti niso:**

- Napačen ključ za shranjevanje v modulu zaupanja TPM, ki je povezan z napravo ob registraciji (preverite KeySignTest med izvajanjem povišane vrednosti)
- Nadomestni ID za prijavo
- Proxyja HTTP ni bilo mogoče najti

Če želite odpraviti težave z ukazom» dsregcmd «, glejte [stanje SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
