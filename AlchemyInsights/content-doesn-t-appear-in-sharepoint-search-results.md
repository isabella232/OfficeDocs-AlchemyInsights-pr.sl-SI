---
title: Vsebina ni prikazana v SharePoint rezultatih iskanja
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081626"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Vsebina ni prikazana v SharePoint rezultatih iskanja

Upoštevajte ta navodila za odpravljanje težav, če pričakovana vsebina ni prikazana v rezultatih iskanja:
  
1. Preverite, ali **je mesto** s pričakovano vsebino nastavljeno tako, da dovoli, da je vsebina prikazana v rezultatih iskanja. Upoštevajte navodila v [koraku Prikaz vsebine na spletnem mestu v rezultatih iskanja.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)

2. Preverite, ali **je seznam** ali **knjižnica,** ki vsebuje pričakovano vsebino, nastavljena tako, da dovoli, da se vsebina prikaže v rezultatih iskanja. Upoštevajte navodila v [članku Prikaz vsebine seznamov ali knjižnic v rezultatih iskanja.](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)

3. Prepričajte se, da je postavitev strani, dokumenta ali strani po meri objavljena kot **glavna različica.** Upoštevajte 3. [korak v možnosti Iskanje ne vrne vseh rezultatov v SharePoint Online.](https://go.microsoft.com/fwlink/?linkid=874525)

4. Preverite, ali ima **uporabnik dovoljenja** za ogled vsebine. Upoštevajte navodila v [razdelku Razumevanje ravni dovoljenj v SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
    
5. Če je bila shema iskanja spremenjena z dodajanjem nove upravljane lastnosti, z urejanjem upravljane lastnosti ali z odstranitvijo upravljane lastnosti, boste morali zahtevati iskanje po vsebini in ponovno indeksiranje. **Znova indeksijte** vsebino tako, da sledite korakom v ročna zahteva iskanja po vsebini in ponovno [indeksiranje mesta, knjižnice ali seznama.](https://docs.microsoft.com/sharepoint/crawl-site-content) To lahko traja nekaj časa, počakajte 24 ur, preden znova preverite rezultate.

Če želite več informacij, glejte [Omogočanje vsebine mesta za iskanje.](https://docs.microsoft.com/sharepoint/make-site-content-searchable) 
  
