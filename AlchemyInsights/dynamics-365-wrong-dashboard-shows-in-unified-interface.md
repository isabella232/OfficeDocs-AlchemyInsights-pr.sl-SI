---
title: Dynamics 365 – napačna nadzorna plošča je prikazana v poenotenem vmesniku storitve Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101498"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Napačna nadzorna plošča je prikazana v poenotenem vmesniku storitve Dynamics 365

Obstaja več razlogov, zakaj morda vidite drugačno nadzorno ploščo od pričakovane:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Uporabnik je nastavil privzeto nadzorno ploščo uporabnika 

Običajno lahko določite privzeto nadzorno ploščo uporabnika, ki je nastavljena, če gumb Nastavi kot **privzeto** ni v ukazni vrstici nadzorne plošče. Privzeta nadzorna plošča uporabnika preglasi vse druge privzete nadzorne plošče, tudi če uporabnikova privzeta nadzorna plošča ni v trenutni aplikaciji.

Če želite odmnoti privzeto nadzorno ploščo, uporabite to rešitev.

1. Ustvarite novo osebno nadzorno ploščo.

2. To novo nadzorno ploščo nastavite kot privzeto uporabnika.

3. Izbrišite to nadzorno ploščo.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Nadzorna plošča je nastavljena v zemljevidu mesta

Morda ste v organizaciji nastavili privzeto nadzorno ploščo tako, da ste izbrali nadzorno ploščo in v razdelku »Prilagajanje sistema« izbrali »Nastavi kot privzeto«. Toda nadzorna plošča, določena v načrtovalniku zemljevidov mesta, ima prednost pred to nadzorno ploščo, če ima uporabnik dostop do te nadzorne plošče.

Če želite, da uporabniki vidijo nadzorno ploščo, ki ste jo nastavili kot privzeto organizacijo, lahko:

* Nastavitev nadzorne plošče v zemljevidu mesta

* Odstranjevanje dostopa do določene nadzorne plošče zemljevida mesta za te uporabnike
