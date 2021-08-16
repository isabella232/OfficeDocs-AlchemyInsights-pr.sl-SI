---
title: Odpravljanje težav z napredno zaščito pred grožnjami Windows 10 Microsoft Defender na daljavo
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
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034050"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Odpravljanje težav z napredno zaščito pred grožnjami Windows 10 Microsoft Defender na daljavo

Če lahko dostopate do oddaljenega računalnika, sledite tem korakom:

1. Prenesite diagnostično [orodje analizatorja povezljivosti](https://go.microsoft.com/fwlink/?linkid=2143466) odjemalca.
2. Izvlečenje in zagon datoteke MDATPAnalyzer.cmd.
3. Poiščite diagnostični dnevnik v mapi MDATPClientAnalyzerResult, ki je ista mapa, v katero je bilo preneseno orodje Analizator.
4. Če želite poiskati težave s povezljivostjo ali nastavitvami internetnega proxyja, preglejte dnevnik MDATPClientAnalyzer.txt.

Če želite izvedeti več, glejte [Težave s računalniki za upravljanje.](https://go.microsoft.com/fwlink/?linkid=2143634)
