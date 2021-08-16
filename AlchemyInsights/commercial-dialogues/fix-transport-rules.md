---
title: Popravljanje prenosnih pravil
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034770"
---
# <a name="fix-transport-rules"></a>Popravljanje prenosnih pravil

Na to sporočilo je vplivalo pravilo toka pošte po meri. Če želite pregledati natančno pravilo, naredite to:

1. Pri rezultatih pošiljanja si v **razdelku Dodatne informacije** **zabeležite GUID** ali ime **pravilnika.**
2. Zaženite Exchange za upravljanje. Če želite več informacij, glejte [Odpiranje ukazne lupine Exchange za upravljanje sistema .](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Zaženite ta ukaz (z UUID iz pošiljanja):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Preglejte opis in si oglejte konfigurirane pogoje, v katere je to sporočilo vplivalo.

Če želite izvedeti več, [glejte Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
