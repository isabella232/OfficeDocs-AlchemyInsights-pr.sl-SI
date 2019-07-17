---
title: Dynamics 365 - narobe armaturni plošči kaže v enotni vmesniku Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748759"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Narobe armaturni plošči kaže v enotni vmesniku Dynamics 365

Obstaja več razlogov, zakaj lahko vidite različne nadzorne plošče kot tisti, ki pričakujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Uporabnik je nastavite privzeti uporabniški nadzorni plošči 

Običajno lahko prepoznavanje uporabnika privzeto nadzorno ploščo je nastavljena, če **Nastavite kot privzeti** gumb ne Prikaži v blatnik ukazno vrstico. Privzete nadzorne plošče uporabnika bo razveljavila vse druge privzete nadzorne plošče, tudi če uporabnikove privzete nadzorne plošče ni v trenutni app.

Raba sledeč workaround v izključeno njihovo privzeto nadzorno ploščo.

1. Ustvarite novo osebno armaturno ploščo.

2. Nastavite to novo nadzorno ploščo kot uporabniško privzeto.

3. Brisanje te nadzorne plošče.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Armaturni plošči se nahaja v kazalo

Lahko nastavite za organizacijo privzeto nadzorno ploščo z izbiro nadzorno ploščo in izberete "Nastavi kot privzeto" pod "Šega sistem". Vendar blatnik, opredeljen v kazalo oblikovalec hoteti zalotiti predhodnost nad to nadzorno ploščo, če uporabnik ima dostop do njega.

Da imajo uporabniki videli armaturni plošči, ki ste jo nastavili kot privzeti organizacije, lahko bodisi:

* Nastavite to nadzorno ploščo v kazalo

* Odstranjevanje dostopa do kazalo določene nadzorne plošče za tiste uporabnike
