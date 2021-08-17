---
title: Single-Sign za naprave Azure Active Directory včlanjene v računalnik
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: 365225926296677feb7853481651a634792fd8bfa9abd9dc9359ffaae50b60eb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050026"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Enotna prijava za naprave, Azure Active Directory pridružene naprave

Če imate okolje imenika Active Directory (AD) na mestu uporabe in želite svoje računalnike, pridružene domeni AD, pridružiti imeniku Azure AD, lahko to dosežete tako, da izvedete hibridno pridružitev imeniku Azure AD. [Kako: načrtujte hibridno združevanje Azure Active Directory vam](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ponuja povezane korake za izvedbo hibridne pridružine storitve Azure AD v vašem okolju.

[Konfiguracija naprav, ki so pridružene imeniku Azure AD, Single-Sign Na mestu uporabe Windows Hello za podjetja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Težave s primarnim žetonom za osveževanje (PRT)** Primarni žeton za osveževanje (PRT) je ključni element preverjanja pristnosti imenika Azure AD v napravah s storitvami Windows 10, Windows Server 2016 in novejšimi različicami ter napravami s sistemom iOS in Android. Gre za žeton JSON Web Token (JWT), ki je posebej izdan Microsoftovim žetonom prve stranke, da omogoči enotno prijavo (SSO) v programih, ki se uporabljajo v teh napravah. [V oknu Kaj je primarni žeton](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)za osveževanje? bomo objavili podrobnosti o tem, kako se izda, uporablja in zaščiti PRT Windows 10 napravah.

**WamDefaultSet: DA in AzureADPrt: DA** Ta polja označujejo, ali je uporabnik ob vpisu v napravo uspešno preverjal pristnost imenika Azure AD. Če so vrednosti **»NO),** lahko zapadejo:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- Nadomestni ID za prijavo
- STREŽNIKA HTTP Proxy ni bilo mogoče najti

Odpravljanje težav z uporabo ukaza dsregcmd – [stanje SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
