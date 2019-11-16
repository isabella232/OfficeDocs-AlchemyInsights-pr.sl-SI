---
title: Dynamics 365-napačna Nadzorna plošča kaže v Dynamics 365 poenoteni vmesnik
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528567"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Napačna Nadzorna plošča je prikazana v poenotenem vmesniku Dynamics 365

Obstaja več razlogov, zakaj se lahko prikaže drugačna Nadzorna plošča kot tista, ki jo pričakujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Uporabnik je nastavil privzeto nadzorno ploščo uporabnika 

Značilno je, da lahko prepoznate uporabniško privzeto nadzorno ploščo je nastavljena, če se **Nastavi kot privzeto** gumb ne prikaže v ukazni vrstici nadzorne plošče. Privzeta Nadzorna plošča za uporabnika bo preglasitev vseh drugih privzetih nadzornih plošč, tudi če uporabnikova privzeta Nadzorna plošča ni v trenutni aplikaciji.

Če želite razdružiti privzeto nadzorno ploščo, uporabite to rešitev.

1. Ustvarite novo osebno nadzorno ploščo.

2. Nastavite novo nadzorno ploščo kot privzeti uporabnik.

3. Izbrišite nadzorno ploščo.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Nadzorna plošča je nastavljena na kazalo

Morda ste nastavili privzeto nadzorno ploščo organizacije tako, da izberete nadzorno ploščo in izberete» Nastavi kot privzeto «pod možnostjo» prilagodi sistem «. Vendar pa bo Nadzorna plošča, določena v Oblikovalniku kazalo, prevladala nad to nadzorno ploščo, če ima uporabnik dostop do njega.

Če želite, da bodo uporabniki videli nadzorno ploščo, ki ste jo nastavili kot privzeto organizacijo, lahko:

* Nastavitev nadzorne plošče na zemljevidu

* Odstranitev dostopa do zemljevida, ki je določena za te uporabnike
