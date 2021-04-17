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
# <a name="cdn-used-for-video-playback"></a>Za predvajanje videoposnetka je uporabljen sistem CDN

Za dogodke v živo v storitvi Stream ter dogodke v živo v zunanji aplikaciji ali napravi v aplikaciji Yammer/Teams, bo samodejno uporabljen Azure CDN. Za predvajanje videoposnetkov na zahtevo, naloženih v aplikacijo Stream, še ni uporabljen sistem Azure CDN. Videoposnetki v storitvi Stream, ki niso predvajani v živo, so predvajani z izvornega strežnika Azure Media Services, povezanega z vašim najemnikom v geografski regiji vašega najemnika. Če želite več informacij, si oglejte:

- [Za predvajanje videoposnetka je uporabljen sistem CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
