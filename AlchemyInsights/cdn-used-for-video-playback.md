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
ms.openlocfilehash: 399be421994437d4cd2df644531334c58d177ec3293e7e379d84cd8326823a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54071132"
---
# <a name="cdn-used-for-video-playback"></a>Za predvajanje videoposnetka je uporabljen sistem CDN

Za dogodke v živo v storitvi Stream ter dogodke v živo v zunanji aplikaciji ali napravi v aplikaciji Yammer/Teams, bo samodejno uporabljen Azure CDN. Za predvajanje videoposnetkov na zahtevo, naloženih v aplikacijo Stream, še ni uporabljen sistem Azure CDN. Videoposnetki v storitvi Stream, ki niso predvajani v živo, so predvajani z izvornega strežnika Azure Media Services, povezanega z vašim najemnikom v geografski regiji vašega najemnika. Če želite več informacij, si oglejte:

- [Za predvajanje videoposnetka je uporabljen sistem CDN](https://docs.microsoft.com/stream/network-overview#cdn-used-for-video-playback)
