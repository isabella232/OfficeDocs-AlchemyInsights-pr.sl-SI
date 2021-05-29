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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702142"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="b4cba-102">Micro zamude ali omejevanje storitve PowerShell v storitvi Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b4cba-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="b4cba-103">Ko zaženete skripte in ukaze »cmdlet« v storitvi Exchange Online, boste morda opazili opozorila »Micro delay applied«.</span><span class="sxs-lookup"><span data-stu-id="b4cba-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="b4cba-104">Tukaj je nekaj predlogov, kako odpraviti to težavo:</span><span class="sxs-lookup"><span data-stu-id="b4cba-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="b4cba-105">Zaženite diagnostiko, da sprostite najemnika pravilnike o zmogljivosti zmogljivosti PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b4cba-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="b4cba-106">S to rešitvijo boste težavo večino rešili.</span><span class="sxs-lookup"><span data-stu-id="b4cba-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="b4cba-107">Če težave še vedno ne odpravite, uporabite modul [Exchange Online v2 PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ki vključuje ukaze CMDlet, ki temeljijo na vmesniku API REST in so znatno bolj učinkovitejši.</span><span class="sxs-lookup"><span data-stu-id="b4cba-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="b4cba-108">To je lahko odlična rešitev za veliko število ukazov» dobi «, ki se pogosto uporabljajo.</span><span class="sxs-lookup"><span data-stu-id="b4cba-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="b4cba-109">Če morate uporabiti ukaze CMDlet, ki niso zajeti v modulu v2, glejte Zagon ukazov [»cmdlet«](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)lupine PowerShell za večje število uporabnikov v programu Office 365, ki govori o tem, kako se lahko v modulu PowerShell omejijo omejevanje zmogljivosti v Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b4cba-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
