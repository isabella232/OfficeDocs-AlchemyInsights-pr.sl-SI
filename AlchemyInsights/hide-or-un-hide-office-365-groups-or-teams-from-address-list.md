---
title: Skrivanje ali skrivanje skupin ali ekip v storitvi Office 365 na seznamu naslovov
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811472"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrivanje ali skrivanje skupin ali ekip v storitvi Office 365 na seznamu naslovov

Uporabite ta ukaz EXO PowerShell, da skrijete ali počistite skupino/ekipe storitve Office 365 na seznamih naslovov (GAL) odjemalcev za Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

S tem ukazom EXO PowerShell skrijte ali počistite skupino/ekipe storitve Office365 v odjemalcih strežnika Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Če želite podrobna navodila, glejte [Skrivanje skupin v storitvi Office 365 v odjemalcih gal in Exchange.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
