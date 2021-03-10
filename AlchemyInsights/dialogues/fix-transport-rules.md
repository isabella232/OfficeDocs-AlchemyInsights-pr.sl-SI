---
title: Popravljanje pravil prenosa
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695862"
---
# <a name="fix-transport-rules"></a>Popravljanje pravil prenosa

To sporočilo je vplivalo na pravilo za tok pošte po meri. Če želite pregledati točno pravilo, naredite to:

1. V razdelku Rezultati pošiljanja v razdelku **dodatne informacije** si zapomnite **GUID** ali **ime pravilnika**.
2. Zaženite ukazno lupino za upravljanje Exchangea. Če želite več informacij, glejte [odpiranje lupine za upravljanje Exchangea](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Zaženite ta ukaz (z GUID-om iz vaše oddaje):  **TransportRule-Identity "GUID" | FL * opis***
4. Če si želite ogledati konfigurirane pogoje, ki so vplivali na sporočilo, preglejte opis.

Če želite izvedeti več, glejte [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
