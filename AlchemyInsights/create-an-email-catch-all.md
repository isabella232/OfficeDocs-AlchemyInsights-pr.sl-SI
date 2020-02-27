---
title: Ustvarite e-poštni ulov vse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286307"
---
# <a name="create-an-email-catch-all"></a>Ustvarite e-poštni ulov vse

Uporaba ulova je vse močno odvrnilo. Bolje je, da zagotovi Odklonijo nazaj pošiljatelju dajanje v najem pošiljatelji vedo svoje sporočilo ni bilo mogoče dostaviti, kot je naslovljena, tako da lahko ukrepajo. Nadzornem nabiralniku lahko omejite tudi na samo ulov prej veljavnih e-poštnih naslovov. 

Vsak ulov vse nabiralnik bo prejel veliko spam in lahko sčasoma izpolnite, če ne pozorno spremljati. (Obstajajo omejitve, ki prejemajo.) 

Če se odločite za nadaljevanje, sledite tem korakom:

1. Ustvarite dinamično distribucijsko skupino & vključujejo» vse vrste prejemnikov «.

2. Ustvarite namenski nabiralnik za ulov e-poštnih sporočil, na primer catchall@domain.com.

3. Za določeno domeno nastavite DomainType na "Internrelay". Če vi slej premestitev zgrabiti vsi, obstati varen v število enakih oseb področje prislon v verodostojni.

4. Ustvarite pravilo za prenos poštnega toka na naslednji način:

    - Če je pošiljatelj "zunaj organizacije"
    - Preusmeri sporočilo na Catchall@domain.com
    - Razen če je prejemnik član allusers@domain.com (distribucijska skupina vsebuje vse člane)
    - Preverite, ali so novi nabiralniki dodani v dinamično distribucijsko skupino
