---
title: Popravljanje pravilnika o povezavi
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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988152"
---
# <a name="fix-connection-policy"></a>Popravljanje pravilnika o povezavi

E-pošta je bila označena kot varna in dostavljena v uporabnikovo mapo »Prejeto«, ker je bil naslov IP za pošiljanje označen kot varen v pravilniku filtra povezave. Če želite pregledati pravilnik, naredite to:

1. Obiščite središče [za Office 365 za zagotavljanje &](https://go.microsoft.com/fwlink/p/?linkid=2077143)s predpisi in pojdite na Pravilnik za upravljanje groženj  >    >  [– neželena pošta](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Na **zavihku** Po meri izberite **pravilnik filtra povezave in** nato uredi **pravilnik.**
3. Preglejte **seznam allow (Dovoljeni naslovi IP).** Oglejte **si Sef ali je** seznam omogočen.

    > [!NOTE]
    > Microsoft se naroči na vire zaupanja vrednih pošiljateljev tretjih oseb. Če **Sef seznam** omogočen, ti zaupanja vredni pošiljatelji niso pomotoma označeni kot neželena pošta. Priporočamo, da izberete to možnost, saj se s tem zmanjša število napačnih pozitivnih pošiljateljev (dobra pošta, ki je razvrščena kot neželena pošta), ki jo prejmete.
