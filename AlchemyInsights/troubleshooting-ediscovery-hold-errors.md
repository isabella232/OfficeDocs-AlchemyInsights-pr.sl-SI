---
title: Pri odpravljanju težav z e-odkrivanjem pride do napak
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676283"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="3b860-102">Pri odpravljanju težav z e-odkrivanjem pride do napak</span><span class="sxs-lookup"><span data-stu-id="3b860-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="3b860-103">Ali imate težave z zadržanjem e-odkrivanja?</span><span class="sxs-lookup"><span data-stu-id="3b860-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="3b860-104">Tukaj je nekaj najboljših praks, na voljo:</span><span class="sxs-lookup"><span data-stu-id="3b860-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="3b860-105">Preverite stanje zadržanja porazdelitve.</span><span class="sxs-lookup"><span data-stu-id="3b860-105">Check the hold distribution status.</span></span>  <span data-ttu-id="3b860-106">Če je stanje **»Izklopljeno« (v čakanju)** ali **»Izklopljeno« (v čakanju),** počakajte, da se porazdelitev konča.</span><span class="sxs-lookup"><span data-stu-id="3b860-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="3b860-107">Spojite posodobitve zadržanja e-odkrivanja v eno množično zahtevo, namesto da bi večkrat posodobili pravilnik za vsako transakcijo.</span><span class="sxs-lookup"><span data-stu-id="3b860-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="3b860-108">Zaženite Set-CaseHoldPolicy <policyname> -RetryDistribution v Powershell središču za varnost in skladnost s predpisi.</span><span class="sxs-lookup"><span data-stu-id="3b860-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="3b860-109">Podrobnosti najdete v Povezovalnik [PowerShell v središču za & in skladnost s predpisi.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="3b860-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="3b860-110">Če želite navodila za preverjanje teh nastavitev in dodatnih najboljših praks za omiljenje in odpravljanje težav z e-odkrivanjem, glejte Odpravljanje napak zadržanja [e-odkrivanja.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="3b860-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="3b860-111">Če želite več informacij o odpravljanju drugih pogostih težav z e-odkrivanjem, glejte Raziščite, odpravite pogoste težave [z e-odkrivanjem](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)in jih odpravite.</span><span class="sxs-lookup"><span data-stu-id="3b860-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
