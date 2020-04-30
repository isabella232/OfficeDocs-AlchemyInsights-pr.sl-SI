---
title: Micro zamude ali omejevanje storitve PowerShell v storitvi Exchange Online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948031"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro zamude ali omejevanje storitve PowerShell v storitvi Exchange Online

Ko zaženete skripte in ukaze »cmdlet« v storitvi Exchange Online, boste morda opazili opozorila »Micro delay applied«. Na voljo sta dva predloga, povezana s tem:

- Morda boste želeli uporabiti modul PowerShell za [Exchange Online v2](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), ki vključuje ukaze »CMDlet«, ki temeljijo na storitvi API REST in so precej bolj izvajani. To je lahko odlična rešitev za veliko število ukazov» dobi «, ki se pogosto uporabljajo.
- Če morate uporabiti ukaze »CMDlet«, ki niso zajeti v modulu v2, si oglejte [zagon ukazov » cmdlet« lupine PowerShell za veliko število uporabnikov v sistemu Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), ki govori o tem, kako se prepričate, da so v storitvi Exchange Online na voljo omejitve omejevanja delovanja lupine PowerShell.
