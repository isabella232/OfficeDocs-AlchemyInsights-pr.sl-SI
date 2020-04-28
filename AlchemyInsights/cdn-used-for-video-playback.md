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
# <a name="cdn-used-for-video-playback"></a>Za predvajanje videoposnetka je uporabljen sistem CDN

Za dogodke v živo v storitvi Stream ter dogodke v živo v zunanji aplikaciji ali napravi v aplikaciji Yammer/Teams, bo samodejno uporabljen Azure CDN. Za predvajanje videoposnetkov na zahtevo, naloženih v aplikacijo Stream, še ni uporabljen sistem Azure CDN. Videoposnetki v storitvi Stream, ki niso predvajani v živo, so predvajani z izvornega strežnika Azure Media Services, povezanega z vašim najemnikom v geografski regiji vašega najemnika. Če želite več informacij, si oglejte:

- [Za predvajanje videoposnetka je uporabljen sistem CDN](https://docs.microsoft.com/sl-SI/stream/network-overview#cdn-used-for-video-playback)
