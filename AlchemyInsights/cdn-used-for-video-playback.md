---
title: Za predvajanje videoposnetka je uporabljen sistem CDN
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002552"
- "5146"
ms.openlocfilehash: 489e92ad8fb38ff6f62db3cb65bfd6d329c63490
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790203"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="187bb-102">Za predvajanje videoposnetka je uporabljen sistem CDN</span><span class="sxs-lookup"><span data-stu-id="187bb-102">CDN used for video playback</span></span>

<span data-ttu-id="187bb-103">Za dogodke v živo v storitvi Stream ter dogodke v živo v zunanji aplikaciji ali napravi v aplikaciji Yammer/Teams, bo samodejno uporabljen Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="187bb-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="187bb-104">Za predvajanje videoposnetkov na zahtevo, naloženih v aplikacijo Stream, še ni uporabljen sistem Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="187bb-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="187bb-105">Videoposnetki v storitvi Stream, ki niso predvajani v živo, so predvajani z izvornega strežnika Azure Media Services, povezanega z vašim najemnikom v geografski regiji vašega najemnika.</span><span class="sxs-lookup"><span data-stu-id="187bb-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="187bb-106">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="187bb-106">For more information, see:</span></span>

- [<span data-ttu-id="187bb-107">Za predvajanje videoposnetka je uporabljen sistem CDN</span><span class="sxs-lookup"><span data-stu-id="187bb-107">CDN used for video playback</span></span>](https://docs.microsoft.com/sl-SI/stream/network-overview#cdn-used-for-video-playback)
