---
title: Uporaba pravilnika DLP v pravilih prenosa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915294"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="f3a08-102">Uporaba pravilnika DLP v pravilih prenosa</span><span class="sxs-lookup"><span data-stu-id="f3a08-102">Using DLP in transport rules</span></span>

<span data-ttu-id="f3a08-103">Če želite preprečitev izgube podatkov (DLP) vgraditi v obstoječi prenos, v nastavitvah pravila prenosa uporabite pogoj »**Če so v sporočilu...občutljive informacije**«.</span><span class="sxs-lookup"><span data-stu-id="f3a08-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="f3a08-104">**Če želite dodatne podrobnosti, glejte:**</span><span class="sxs-lookup"><span data-stu-id="f3a08-104">**For more details, see:**</span></span>

- <span data-ttu-id="f3a08-105">Vgrajene vrste občutljivih informacij DLP v pravilih prenosa: [Vgraditev pravil o občutljivih informacijah](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="f3a08-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="f3a08-106">Pravilo lahko preizkusite tudi s preizkusom pravilnika ali brez njega tako, da za pravilo uporabite način preizkusa.</span><span class="sxs-lookup"><span data-stu-id="f3a08-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="f3a08-107">Ko ustvarite pravilo, počakajte 30 minut, preden ga preizkusite.</span><span class="sxs-lookup"><span data-stu-id="f3a08-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="f3a08-108">Glejte [Preizkus pravil za tok pošte/prenos](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="f3a08-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="f3a08-109">**Opomba**: če skušate v EAC uvesti nov pravilnik DLP s pravili prenosa, namesto tega uporabite [pravilnike DLP v središču za varnost in skladnost s predpisi](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="f3a08-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
