---
title: Pozdravno sporočilo v Microsoftovih 365 skupinah
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358337"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Pozdravno sporočilo v Microsoftovih 365 skupinah

Novi uporabniki, ki se pridružijo skupini Microsoft 365, prejmejo pozdravno e-poštno sporočilo, če je lastnost» UnifiedGroupWelcomeMessageEnabled «resnična.

V primeru, da želite onemogočiti pozdravno sporočilo, uporabite ta ukaz [exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) :

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
