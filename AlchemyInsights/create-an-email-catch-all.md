---
title: Ustvarjanje e-poštnega sporočila »Zasuti vse«
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816216"
---
# <a name="create-an-email-catch-all"></a>Ustvarjanje e-poštnega sporočila »Zasuti vse«

Uporaba catch all is strongly discouraged. Pošiljatelju raje pošljite sporočilo o tem, da sporočila ni bilo mogoče dostaviti kot obravnavano, zato da lahko ukrepajo. Nadzorujete lahko tudi nabiralnik, ki ste ga spremljali, in tako omejite, da v preteklosti velja le za veljavne e-poštne naslove. 

Vsaka zaseda vse nabiralnike prejme veliko neželene pošte in bo sčasoma lahko zapolnila, če ne bo skrbno nadzorovana. (Omejitve prejemanja.) 

Če želite nadaljevati, upoštevajte ta navodila:

1. Ustvarite dinamično skupino prejemnikov, & »All Recipient Types« (Vse vrste prejemnikov).

2. Ustvarite namenski nabiralnik, da zasukate e-poštna sporočila, na primer catchall@domain.com.

3. Za določeno domeno nastavite DomainType na »InternalRelay«. Če pozneje odstranite catch all (zajemi), ne glede na to, ali ste domeno nastavili nazaj na Avtoritativno.

4. Prenosno pravilo za poštni tok ustvarite tako:

    - Če je pošiljatelj »Zunaj organizacije«
    - Preusmeri sporočilo v Catchall@domain.com
    - Razen če je prejemnik član skupine allusers@domain.com (skupina prejemnikov vsebuje vse člane)
    - Preverite, ali so novi nabiralniki dodani v dinamično skupino prejemnikov
