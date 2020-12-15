---
title: Samodejno vpis v Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678816"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Samodejno vpis v Microsoft Edge

Microsoft Edge uporablja privzeti račun OS za samodejno vpis uporabnika glede na to, kako je uporabnikova naprava konfigurirana. 

Scenariji za vsako vrsto konfiguracije naprave in njegovega odvisnega postopka za vpis uporabnika so opisani spodaj:

1. **Naprava je hibridna/zvočna – J**: Ta možnost je na voljo v sistemu Windows 10, sistemu Windows in ustreznih različicah strežnika. Uporabniki so samodejno vpisani s svojimi računi v storitvi Azure Active Directory (AD).
2. **Naprava je povezana z domeno**: Ta možnost je na voljo v sistemu Windows 10, sistemu Windows in ustreznih različicah strežnika. Uporabniki z računi domene privzeto niso samodejno vpisani; Če želite omogočiti samodejno vpis, uporabite pravilnik **ConfigureOnPremisesAccountAutoSignIn** . Če želite omogočiti samodejno vpis za uporabnike z računi Azure AD, razmislite o hibridnih pridruževanju svojih naprav.
3. **Privzeti račun za OS je Microsoftov račun**: Ta možnost je na voljo v sistemu Windows 10 RS3 (različica 1709, graditev 10.0.16299) in novejših različicah. V napravah za podjetja ni verjetno, da bi prišlo do scenarija. Če pa je privzeti račun za OS Microsoftov račun, se Microsoft Edge samodejno vpiše v uporabnika z Microsoftovim računom.
 
 
