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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="3aa09-102">Skrivanje ali skrivanje skupin ali ekip v storitvi Office 365 na seznamu naslovov</span><span class="sxs-lookup"><span data-stu-id="3aa09-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="3aa09-103">Uporabite ta ukaz EXO PowerShell, da skrijete ali počistite skupino/ekipe storitve Office 365 na seznamih naslovov (GAL) odjemalcev za Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="3aa09-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="3aa09-104">S tem ukazom EXO PowerShell skrijte ali počistite skupino/ekipe storitve Office365 v odjemalcih strežnika Exchange (Outlook, OWA):</span><span class="sxs-lookup"><span data-stu-id="3aa09-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="3aa09-105">Če želite podrobna navodila, glejte [Skrivanje skupin v storitvi Office 365 v odjemalcih gal in Exchange.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)</span><span class="sxs-lookup"><span data-stu-id="3aa09-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
