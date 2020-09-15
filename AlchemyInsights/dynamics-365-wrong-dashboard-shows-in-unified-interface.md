---
title: Dynamics 365 – napačna Nadzorna plošča v dinamiki 365 Unified Interface
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
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711291"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Napačna Nadzorna plošča v sistemu Dynamics 365 Unified Interface

Obstaja več razlogov, zakaj se lahko prikaže druga Nadzorna plošča, kot je tista, ki jo pričakujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Uporabnik je nastavil privzeto nadzorno ploščo uporabnika 

Običajno lahko prepoznate privzeto nadzorno ploščo uporabnika, če gumb» **Nastavi kot privzeto** «ni prikazan v ukazni vrstici nadzorne plošče. Privzeta Nadzorna plošča uporabnika bo preglasila vse druge privzete nadzorne plošče, tudi če uporabnikove privzete nadzorne plošče ni v trenutni aplikaciji.

Če želite izključiti privzeto nadzorno ploščo, uporabite to nadomestno rešitev.

1. Ustvarite novo osebno nadzorno ploščo.

2. Nastavite to novo nadzorno ploščo kot privzeti uporabnik.

3. Izbrišite to nadzorno ploščo.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Nadzorna plošča je nastavljena v kazalo

Morda ste nastavili privzeto nadzorno ploščo organizacije tako, da izberete nadzorno ploščo in izberete možnost» Nastavi kot privzeto «v razdelku» prilagodi sistem «. Nadzorna plošča, ki je opredeljena v Oblikovalniku zemljevida sitemap, bo imela prednost pred to nadzorno ploščo, če ima uporabnik dostop do njega.

Če želite, da uporabniki vidijo nadzorno ploščo, ki ste jo nastavili kot privzeto organizacijo, lahko naredite to:

* Nastavitev nadzorne plošče v sitemap

* Odstranjevanje dostopa do določene nadzorne plošče za kazalo za te uporabnike
