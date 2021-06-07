---
title: Težave z učinkovitostjo delovanja za Microsoft Defender za končno točko v sistemu Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794226"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="5759b-102">Težave z učinkovitostjo delovanja za Microsoft Defender za končno točko v sistemu Linux</span><span class="sxs-lookup"><span data-stu-id="5759b-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="5759b-103">V tem članku so navodila za določanje težav z učinkovitostjo delovanja za Microsoft Defender for Endpoint v sistemu Linux.</span><span class="sxs-lookup"><span data-stu-id="5759b-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="5759b-104">Pomembno je, da najprej preverite, ali je težava, do katere prihaja, odpravljena z [najnovejšo različico.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="5759b-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="5759b-105">Če želite začeti raziskovanje, glejte Odpravljanje [težav z učinkovitostjo delovanja za Microsoft Defender for Endpoint v sistemu Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="5759b-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="5759b-106">Izključitve</span><span class="sxs-lookup"><span data-stu-id="5759b-106">Exclusions</span></span>

<span data-ttu-id="5759b-107">Z izključitevm lahko zmanjšate težave z učinkovitostjo delovanja.</span><span class="sxs-lookup"><span data-stu-id="5759b-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="5759b-108">Preden začnete, preglejte izključitve, da bo vsa dodatna tveganja znana in dokumentirana.</span><span class="sxs-lookup"><span data-stu-id="5759b-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="5759b-109">Če želite več informacij, glejte [Konfiguracija in preverjanje veljavnosti izključitev za Microsoft Defender for Endpoint on Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="5759b-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="5759b-110">Če morate izključiti & datotek ali map, ki so vse v isti kopeti, je morda lažje, če izključite točko konjene.</span><span class="sxs-lookup"><span data-stu-id="5759b-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="5759b-111">S februarsko izdajo 101.22.80 lahko izključite celotno točko konjene.</span><span class="sxs-lookup"><span data-stu-id="5759b-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="5759b-112">Če je na primer /mnt/varnostna kopija gora, lahko na izključen seznam dodate /mnt/backup tako, da zaženete ta ukaz:</span><span class="sxs-lookup"><span data-stu-id="5759b-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="5759b-113">**Opomba:** z dodajanjem izključitev povečate tveganje, da zlonamerna programska oprema ne bo zaznana, zato jo morate obravnavati in uvesti previdno.</span><span class="sxs-lookup"><span data-stu-id="5759b-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="5759b-114">Potrebujete pomoč?</span><span class="sxs-lookup"><span data-stu-id="5759b-114">Need Help?</span></span>

<span data-ttu-id="5759b-115">Če želite pomoč na najučinkovitejši način, zberite diagnostične podatke, preden odprete primer podpore.</span><span class="sxs-lookup"><span data-stu-id="5759b-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
