---
title: Za predvajanje videoposnetka je uporabljen sistem CDN
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
- "9002552"
- "5146"
ms.openlocfilehash: d9c5f8f586e7f5aa079b28584375516ec8401ca7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819384"
---
# <a name="cdn-used-for-video-playback"></a><span data-ttu-id="d37ad-102">Za predvajanje videoposnetka je uporabljen sistem CDN</span><span class="sxs-lookup"><span data-stu-id="d37ad-102">CDN used for video playback</span></span>

<span data-ttu-id="d37ad-103">Za dogodke v živo v storitvi Stream ter dogodke v živo v zunanji aplikaciji ali napravi v aplikaciji Yammer/Teams, bo samodejno uporabljen Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="d37ad-103">Live events from Stream and External app or device live events from Yammer/Teams will automatically use Azure CDN.</span></span> <span data-ttu-id="d37ad-104">Za predvajanje videoposnetkov na zahtevo, naloženih v aplikacijo Stream, še ni uporabljen sistem Azure CDN.</span><span class="sxs-lookup"><span data-stu-id="d37ad-104">On-demand videos uploaded to Stream don't yet use Azure CDN for playback.</span></span> <span data-ttu-id="d37ad-105">Videoposnetki v storitvi Stream, ki niso predvajani v živo, so predvajani z izvornega strežnika Azure Media Services, povezanega z vašim najemnikom v geografski regiji vašega najemnika.</span><span class="sxs-lookup"><span data-stu-id="d37ad-105">Non-live videos in Stream are played back from the Azure Media Services origin server associated with your tenant in your tenant's geographic region.</span></span> <span data-ttu-id="d37ad-106">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="d37ad-106">For more information, see:</span></span>

- [<span data-ttu-id="d37ad-107">Za predvajanje videoposnetka je uporabljen sistem CDN</span><span class="sxs-lookup"><span data-stu-id="d37ad-107">CDN used for video playback</span></span>](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
