---
title: Single-Sign v napravah, ki so pridružene imeniku Azure Active Directory
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
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405661"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Enotna prijava za naprave, ki so pridružene imeniku Azure Active Directory

Če imate okolje imenika Active Directory (AD) na mestu uporabe in želite svoje računalnike, pridružene domeni AD, pridružiti imeniku Azure AD, lahko to dosežete tako, da izvedete hibridno pridružitev imeniku Azure AD. [Kako: Načrtujte hibridno združevanje](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) imenika Azure Active Directory vam ponuja sorodne korake za izvedbo hibridne pridružine storitve Azure AD v vašem okolju.

[Konfiguracija naprav, ki so pridružene imeniku Azure AD, za Single-Sign na mestu uporabe: uporaba funkcije Windows Hello za podjetja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Težave s primarnim žetonom za osveževanje (PRT)** Primarni žeton za osveževanje (PRT) je ključni element preverjanja pristnosti imenika Azure AD v sistemih Windows 10, Windows Server 2016 in novejših različicah ter napravah s sistemom iOS in Android. Gre za žeton JSON Web Token (JWT), ki je posebej izdan Microsoftovim žetonom prve stranke, da omogoči enotno prijavo (SSO) v programih, ki se uporabljajo v teh napravah. [V oknu Kaj je primarni](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)žeton za osveževanje? bomo objavili podrobnosti o tem, kako se izda, uporablja in zaščiti PRT v napravah s sistemom Windows 10.

**WamDefaultSet: DA in AzureADPrt: DA** Ta polja označujejo, ali je uporabnik ob vpisu v napravo uspešno preverjal pristnost imenika Azure AD. Če so vrednosti **»NO),** lahko zapadejo:

- Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).
- Nadomestni ID za prijavo
- STREŽNIKA HTTP Proxy ni bilo mogoče najti

Odpravljanje težav z uporabo ukaza dsregcmd – [stanje SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
