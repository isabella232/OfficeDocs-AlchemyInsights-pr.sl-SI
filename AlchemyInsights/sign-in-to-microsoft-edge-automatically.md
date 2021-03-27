---
title: Samodejni vpis v Microsoft Edge
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398745"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Samodejni vpis v Microsoft Edge

Microsoft Edge s privzetim računom operacijskega sistema samodejno vpiše uporabnika glede na to, kako je konfigurirana uporabnikova naprava. 

Scenariji posamezne vrste konfiguracije naprave in odvisni procesi vpisa uporabnikov so opisani spodaj:

- **Naprava je hibridna/AAD-J:** Ta možnost je na voljo v sistemu Windows 10, sistemih Windows navzdol in ustreznih različicah strežnika. Uporabniki so samodejno vpisani s svojimi računi imenika Azure Active Directory (AD).
- **Naprava je pridružena domeni:** Ta možnost je na voljo v sistemu Windows 10, sistemu Windows s ravneh navzdol in ustreznih različicah strežnika. Uporabniki z računi domene privzeto niso vpisani samodejno; če želite omogočiti samodejni vpis zanje, uporabite pravilnik **ConfigureOnPremisesAccountAutoSignIn.** Če želite omogočiti samodejni vpis za uporabnike z računi Azure AD, razmislite o hibridnem pridruževati se svojim napravam.
- Privzeti **račun operacijskega** sistema je Microsoftov račun: ta možnost je na voljo v sistemu Windows 10 RS3 (različica 1709, gradjša 10.0.16299) in novejših različicah. Ta scenarij je malo verjeten za uporabo v napravah podjetja. Če pa je privzeti račun operacijskega sistema Microsoftov račun, se microsoft Edge samodejno vpiše z uporabnikom z Microsoftovim računom.
 
 
