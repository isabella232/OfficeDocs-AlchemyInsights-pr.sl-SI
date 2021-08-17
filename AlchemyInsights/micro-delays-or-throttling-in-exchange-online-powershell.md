---
title: Micro zamude ali omejevanje storitve PowerShell v storitvi Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314716"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro zamude ali omejevanje storitve PowerShell v storitvi Exchange Online

Ko zaženete skripte in ukaze »cmdlet« v storitvi Exchange Online, boste morda opazili opozorila »Micro delay applied«. Tukaj je nekaj predlogov, kako odpraviti to težavo:

- Zaženite diagnostiko, da sprostite najemnika pravilnike o zmogljivosti zmogljivosti PowerShell. S to rešitvijo boste težavo večino rešili.
- Če težave še vedno ne odpravite, uporabite modul [Exchange Online v2 PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ki vključuje ukaze CMDlet, ki temeljijo na vmesniku API REST in so znatno bolj učinkovitejši. To je lahko odlična rešitev za veliko število ukazov» dobi «, ki se pogosto uporabljajo.
- Če morate uporabiti ukaze CMDlet, ki niso zajeti v modulu v2, glejte Izvajanje ukazov [»cmdlet«](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)lupine PowerShell za večje število uporabnikov v programu Office 365, ki govori o tem, kako se lahko v modulu PowerShell omejijo omejevanje zmogljivosti v Exchange Online.
