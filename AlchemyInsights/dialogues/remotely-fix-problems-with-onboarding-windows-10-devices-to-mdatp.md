---
title: Oddaljeno odpravljanje težav z napravami s sistemom Windows 10 za napredna zaščita pred grožnjami
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694845"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Oddaljeno odpravljanje težav z napravami s sistemom Windows 10 za napredna zaščita pred grožnjami

Če lahko dostopate do oddaljenega računalnika, upoštevajte ta navodila:

1. Prenesite diagnostično orodje [analizator povezljivosti odjemalca](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. Ekstrahirajte in zaženite MDATPAnalyzer. cmd.
3. Poiščite diagnostični dnevnik v mapi MDATPClientAnalyzerResult, ki je ista mapa, v kateri je bilo preneseno orodje analizatorja.
4. Če želite poiskati težave s povezljivostjo ali nastavitvami internetnega proxyja, Preglejte dnevniško datoteko MDATPClientAnalyzer.txt.

Če želite izvedeti več, glejte [težave s stroji za vkrcanje](https://go.microsoft.com/fwlink/?linkid=2143634).
