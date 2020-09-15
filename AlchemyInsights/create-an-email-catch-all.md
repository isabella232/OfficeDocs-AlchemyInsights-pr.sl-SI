---
title: Ustvarjanje e-poštnega ulova
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713002"
---
# <a name="create-an-email-catch-all"></a>Ustvarjanje e-poštnega ulova

Uporaba ulova je zelo odvrnjena. Bolje je, da pošljete pošiljateljem, da se ne morejo dostaviti tako, da bodo lahko ukrepali, če želite poslati odklon. Nadzorovani nabiralnik lahko omejite tudi tako, da ujamete le prej veljavne e-poštne naslove. 

Vsak ulov nabiralnika bo prejel dobro ponudbo neželene pošte in lahko sčasoma zapolni, če ni pozorno spremljati. (Obstajajo omejitve za prejemanje.) 

Če se odločite nadaljevati, upoštevajte ta navodila:

1. Ustvarjanje dinamične distribucijske skupine & vključuje» vse vrste prejemnikov «.

2. Ustvarjanje namenskega nabiralnika za lovljenje e-poštnih sporočil, na primer catchall@domain.com.

3. Za določeno domeno nastavite DomainType na» InternalRelay «. Če pozneje odstranite vse, se prepričajte, da je domena nastavljena na avtoritativno.

4. Ustvarite pravilo za prenos Mailflow, kot sledi:

    - Če je pošiljatelj» zunaj organizacije «
    - Preusmeritev sporočila v Catchall@domain.com
    - Razen če je prejemnik član allusers@domain.com (skupina prejemnikov vsebuje vse člane)
    - Preverite veljavnost novih nabiralnikov v dinamični distribucijski skupini.
