---
title: Povezovanje skriptov Lupine PowerShell s strežnikom Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 34301e62a25e11c5d4c353166f8208ef74245dfa
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423778"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="3340d-102">Povezovanje skriptov Lupine PowerShell s strežnikom Exchange Online</span><span class="sxs-lookup"><span data-stu-id="3340d-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="3340d-103">Osnovno preverjanje pristnosti v storitvi Exchange Online bo zastarelo, pot naprej pa je povezovanje s preverjanjem pristnosti na podlagi potrdil za skripte in nespremljana opravila.</span><span class="sxs-lookup"><span data-stu-id="3340d-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="3340d-104">Če želite izvedeti več, [glejte Preverjanje pristnosti samo za aplikacije za nespremljane skripte v modulu EXO V2](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span><span class="sxs-lookup"><span data-stu-id="3340d-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>