---
title: Težave z uvajanje stroji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141661"
---
# <a name="issues-with-onboarding-machines"></a>Težave z uvajanje stroji

Morda imate težave z napravami za vkrcavanje na storitev MDATP. Če lahko dostopate do stroja za končnega uporabnika, sledite tem korakom:

1. Prenesite diagnostično orodje [analizatorja povezljivosti odjemalca](https://aka.ms/mdatpanalyzer) .
2. Citat ter prost dostop MDATPAnalyzer. cmd.
3. Poiščite diagnostični dnevnik v mapi z imenom MDATPClientAnalyzerResult, isto mapo, kjer je orodje za analizo preneseno.
4. Preglejte dnevniško datoteko, MDATPClientAnalyzer.txt, da poiščete težave z nastavitvami povezljivosti ali internetne proxy.