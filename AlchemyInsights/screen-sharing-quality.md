---
title: Kakovost skupne rabe zaslona
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11061"
- "11062"
- "9002254"
- "9002536"
ms.openlocfilehash: 0832f886d3f5c0bfbfe138647403e4e215deaacb
ms.sourcegitcommit: d822377ec76adf9ef6d13bc761a16c9900a3e7cb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/26/2021
ms.locfileid: "52125446"
---
# <a name="screen-sharing-quality"></a><span data-ttu-id="0dbea-102">Kakovost skupne rabe zaslona</span><span class="sxs-lookup"><span data-stu-id="0dbea-102">Screen sharing quality</span></span>

<span data-ttu-id="0dbea-103">V večini primerov pride do težav s kakovostjo zaslona v skupni rabi tako, da je pasovna širina odjemalca omejena.</span><span class="sxs-lookup"><span data-stu-id="0dbea-103">In most cases quality issues with Screen Sharing comes down to limited bandwidth from the client side.</span></span>  <span data-ttu-id="0dbea-104">Kjer pasovna širina ni omejena, Teams optimizira kakovost predstavnosti, vključno z do 1080p ločljivostjo videoposnetka, do 30fps za video in 15fps za vsebino ter zvok visoke ločljivosti.</span><span class="sxs-lookup"><span data-stu-id="0dbea-104">Where bandwidth isn't limited, Teams optimizes media quality, including up to 1080p video resolution, up to 30fps for video and 15fps for content, and high-fidelity audio.</span></span>

<span data-ttu-id="0dbea-105">Teams pri uporabi pasovne širine je vedno pomembno in lahko zagotavlja kakovost videoposnetka HD pod 1,2 Mb/</span><span class="sxs-lookup"><span data-stu-id="0dbea-105">Teams is always conservative on bandwidth utilization and can deliver HD video quality in under 1.2Mbps.</span></span> <span data-ttu-id="0dbea-106">Dejanska poraba pasovne širine za posamezen video- ali zvočni klic ali srečanje se razlikuje glede na dejavnike, kot so postavitev videa, ločljivost videoposnetka in video okvirji na sekundo.</span><span class="sxs-lookup"><span data-stu-id="0dbea-106">The actual bandwidth consumption in each audio/video call or meeting vary based on factors such as video layout, video resolution, and video frames per second.</span></span> <span data-ttu-id="0dbea-107">Ko je na voljo več pasovne širine, se kakovost in uporaba povečata, da zagotovita najboljšo izkušnjo.</span><span class="sxs-lookup"><span data-stu-id="0dbea-107">When more bandwidth is available, quality and usage increase to deliver the best experience.</span></span> <span data-ttu-id="0dbea-108">V tej tabeli je opisano, Teams uporablja pasovno širino:</span><span class="sxs-lookup"><span data-stu-id="0dbea-108">This table describes how Teams uses bandwidth:</span></span>

<span data-ttu-id="0dbea-109">**Scenariji pasovne širine (gor/dol)**</span><span class="sxs-lookup"><span data-stu-id="0dbea-109">**Bandwidth(up/down) Scenarios**</span></span>

- <span data-ttu-id="0dbea-110">30 kb/s Zvočni klici v omrežju enakovrednih</span><span class="sxs-lookup"><span data-stu-id="0dbea-110">30 kbps Peer-to-peer audio calling</span></span>

- <span data-ttu-id="0dbea-111">130 kb/s Zvočni klici v omrežju enakovrednih in skupna raba zaslona</span><span class="sxs-lookup"><span data-stu-id="0dbea-111">130 kbps Peer-to-peer audio calling and screen sharing</span></span>

- <span data-ttu-id="0dbea-112">500 kb/s Videoklici kakovosti v omrežju enakovrednih 360p za 30fps</span><span class="sxs-lookup"><span data-stu-id="0dbea-112">500 kbps Peer-to-peer quality video calling 360p at 30fps</span></span>

- <span data-ttu-id="0dbea-113">1,2 Mb/s Videoklici v ločljivosti HD v omrežju enakovrednih z ločljivostjo HD 720p pri 30fps</span><span class="sxs-lookup"><span data-stu-id="0dbea-113">1.2 Mbps Peer-to-peer HD quality video calling with resolution of HD 720p at 30fps</span></span>

- <span data-ttu-id="0dbea-114">1,5 Mb/s Videoklici v kakovosti v omrežju enakovrednih z ločljivostjo HD 1080p za 30fps</span><span class="sxs-lookup"><span data-stu-id="0dbea-114">1.5 Mbps Peer-to-peer HD quality video calling with resolution of HD 1080p at 30fps</span></span>

- <span data-ttu-id="0dbea-115">Videoklici skupine 500kbps/1Mbps</span><span class="sxs-lookup"><span data-stu-id="0dbea-115">500kbps/1Mbps Group Video calling</span></span>

- <span data-ttu-id="0dbea-116">Videoklici skupine HD 1Mbps/2Mbps (540p videov na zaslonu 1080p)</span><span class="sxs-lookup"><span data-stu-id="0dbea-116">1Mbps/2Mbps HD Group video calling (540p videos on 1080p screen)</span></span>

<span data-ttu-id="0dbea-117">Če želite več informacij, [glejte Priprava omrežja organizacije na Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span><span class="sxs-lookup"><span data-stu-id="0dbea-117">For more information, see [Prepare your organization's network for Microsoft Teams](https://docs.microsoft.com/microsoftteams/prepare-network#bandwidth-requirements)</span></span>