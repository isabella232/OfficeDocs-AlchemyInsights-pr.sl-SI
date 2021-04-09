---
title: Odpravljanje 0x8004de40 v storitvi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649764"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Odpravljanje 0x8004de40 v storitvi OneDrive

Če uporabljate Windows 7 in se prikaže ta napaka, posodobite, da omogočite [TLS 1.1 in TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kot privzete varne protokole v sistemu WinHTTP v sistemu Windows.

Če imate nameščen Windows 10 in se prikaže sporočilo o 0x8004de40 v storitvi OneDrive:

- Ko imate vzpostavljeno povezavo z domeno Acitve Directory, znova zaženite računalnik, v katerem to vpliva.
- Če težave ne odpravite s ponovnim zagonom, se odklopite in se znova pridružite napravi v imeniku Azure AD. 

**Opomba:** V omrežju podjetja morate biti med izvajanjem teh korakov. Teh korakov ne izvedite, če niste povezani s infrastrukturo podjetja (na primer med potovanjem). 

1. Odprite ukazni poziv na skrbniški ravni tako, da izberete **Začetek**, z desno tipko miške kliknite **Ukazni** poziv in nato izberite **Zaženi kot skrbnik**.

1. Vnesite *dsregcmd /leave in* pritisnite **Enter**.

1. Ko končate, vnesite *dsregcmd /join in* pritisnite **tipko Enter**.

1. Ko je ukazni poziv dokončan, ga zaprite.

1. Znova zaženite računalnik in se prijavite v OneDrive.