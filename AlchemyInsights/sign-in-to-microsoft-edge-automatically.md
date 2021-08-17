---
title: Samodejno se vpišite Microsoft Edge vpis
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050710"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Samodejno se vpišite Microsoft Edge vpis

Microsoft Edge uporablja privzeti račun operacijskega sistema za samodejni vpis uporabnika glede na to, kako je uporabnikova naprava konfigurirana. 

Scenariji posamezne vrste konfiguracije naprave in odvisni procesi vpisa uporabnikov so opisani spodaj:

- **Naprava je hibridna/AAD-J:** Ta možnost je na voljo v Windows 10, različicah strežnika Windows in ustreznih različicah strežnika. Uporabniki so samodejno vpisani s svojimi Azure Active Directory (AD).
- **Naprava je pridružena domeni:** ta možnost je na voljo v Windows 10 različicah strežnika, različicah strežnika Windows in ustreznih različicah strežnika. Uporabniki z računi domene privzeto niso vpisani samodejno; če želite omogočiti samodejni vpis zanje, uporabite pravilnik **ConfigureOnPremisesAccountAutoSignIn.** Če želite omogočiti samodejni vpis za uporabnike z računi Azure AD, razmislite o hibridnem pridruževati se svojim napravam.
- **Privzeti račun operacijskega sistema** je Microsoftov račun: ta možnost je na voljo v sistemu Windows 10 RS3 (različica 1709, gradi 10.0.16299) in novejših različicah. Ta scenarij je malo verjeten za uporabo v napravah podjetja. Če pa je privzeti račun operacijskega sistema Microsoftov račun, se Microsoft Edge samodejno vpišete z Microsoftovim računom.
 
 
