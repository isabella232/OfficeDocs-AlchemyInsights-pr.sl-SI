---
title: Odpravljanje težav z enotno prijavo za naprave, ki so pridružene imeniku Azure AD
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
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039262"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Odpravljanje težav z enotno prijavo za naprave, ki so pridružene imeniku Azure AD

Če imate okolje imenika Active Directory (AD) na mestu uporabe in želite svoje računalnike, pridružene domeni AD, pridružiti imeniku Azure AD, lahko to dosežete tako, da izvedete hibridno pridružitev imeniku Azure AD. [Kako: načrtujte hibridno združevanje Azure Active Directory vam](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ponuja povezane korake za izvedbo hibridne pridružine storitve Azure AD v vašem okolju.

Če želite več informacij, glejte [Konfiguracija naprav,](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)ki so pridružene imeniku Azure AD, za Single-Sign na mestu uporabe Windows Hello za podjetja.

**Težave s primarnim žetonom za osveževanje (PRT)**

Primarni žeton za osveževanje (PRT) je ključni element preverjanja pristnosti imenika Azure AD v napravah s storitvami Windows 10, Windows Server 2016 in novejšimi različicami ter napravami s sistemom iOS in Android. Gre za žeton JSON Web Token (JWT), ki je posebej izdan Microsoftovim žetonom prve stranke, da omogoči enotno prijavo (SSO) v programih, ki se uporabljajo v teh napravah. Če želite več informacij o tem, kako se izda, uporablja in ščiti v Windows 10, glejte Kaj je žeton za primarno [osveževanje?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: DA in AzureADPrt: DA**

Ta polja označujejo, ali je uporabnik ob vpisu v napravo uspešno preverjal pristnost imenika Azure AD. Če so vrednosti **»NO),** so lahko posledica:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)
- Nadomestni ID za prijavo
- STREŽNIKA HTTP Proxy ni bilo mogoče najti

Če želite odpraviti težave z napravami z ukazom dsregcmd, glejte [Stanje SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
