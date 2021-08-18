---
title: Skrivanje ali skrivanje vseh skupin Office 365 ekip na seznamu naslovov
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088412"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrivanje ali skrivanje vseh skupin Office 365 ekip na seznamu naslovov

S tem ukazom EXO PowerShell skrijte ali Office 365 skupino/skupine na seznamih naslovov (GAL) odjemalcev Exchange (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

S tem ukazom EXO PowerShell skrijte ali počistite skupino/ekipe storitve Office365 v odjemalcih storitve Exchange (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Če želite podrobna navodila, [glejte Skrivanje Office 365 skupin v gal in Exchange odjemalcih.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
