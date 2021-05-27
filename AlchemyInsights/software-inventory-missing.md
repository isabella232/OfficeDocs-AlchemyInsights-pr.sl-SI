---
title: Zaloga programske opreme manjka ali je netočna
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676515"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="b4eb0-102">Zaloga programske opreme manjka ali je netočna</span><span class="sxs-lookup"><span data-stu-id="b4eb0-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="b4eb0-103">Zaloga programske opreme upravljanje groženj in ranljivosti (TVM) je seznam znane programske opreme v vaši organizaciji z uradnimi skupnimi oštevilčenji platform (CPE).</span><span class="sxs-lookup"><span data-stu-id="b4eb0-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="b4eb0-104">Izdelki programske opreme, ki imajo uradni CPE, imajo objavljene ranljivosti.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="b4eb0-105">Zaloga vključuje tudi podrobnosti, kot so ime dobavitelja, število zalog, groženj in število naprav, ki so izpostavljene.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="b4eb0-106">Spremembe programske opreme v napravah se običajno odrazijo na varnostnih portalih v dveh urah.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="b4eb0-107">Vendar pa lahko včasih traja dlje.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="b4eb0-108">Sinhronizacije trenutno ni mogoče vsiliti; to je stalna ocena.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="b4eb0-109">Če ste spremenili programsko opremo in se sprememba v programu TVM po 5 urah ne odraža natančno, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="b4eb0-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="b4eb0-110">V razdelku z dokaze o programski opremi preverite, kako je bila zaznana programska oprema.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="b4eb0-111">Prepričajte se, da je programska oprema podprta.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-111">Make sure that the software is supported.</span></span> <span data-ttu-id="b4eb0-112">Programska oprema je morda vidna le na ravni naprave, tudi če je trenutno ne podpira upravljanje groženj in ranljivosti.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="b4eb0-113">Vendar pa so na voljo le omejeni podatki.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="b4eb0-114">Če želite navodila za poročanje o točnosti portala, glejte [Nenatančnost poročila.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="b4eb0-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="b4eb0-115">**Opomba:** Poročanje o nenatančni poti portala MDE je prehod iz enega načina v inženirstvo.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="b4eb0-116">Če je težava nujna, odprite vstopnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="b4eb0-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="b4eb0-117">Če želite več informacij, glejte [Zaloga programske opreme – upravljanje groženj in ranljivosti.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="b4eb0-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>