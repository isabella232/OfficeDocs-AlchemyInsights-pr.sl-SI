---
title: Zagon diagnostike pomnilnika sistema Windows v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826683"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Zagon diagnostike pomnilnika sistema Windows v sistemu Windows 10

Če se Windows in aplikacije v računalniku zrušijo, zamrznejo ali delujejo nestabilen, imate morda težave s pomnilnikom računalnika (RAM). Zaženete lahko diagnostiko pomnilnika v sistemu Windows in preverite težave z RAM-om računalnika.

V iskalno polje v opravilni vrstici vnesite **diagnostika pomnilnika** in nato izberite **Diagnostika pomnilnika sistema Windows**. 

Če želite zagnati diagnostiko, morate računalnik znova zagnati. Na voljo je možnost za takojšni vnovični zagon (shranite svoje delo in najprej zaprite dokumente in e-poštna sporočila) ali pa načrtujte samodejno izvajanje diagnostike ob naslednjem ponovnem zagonu računalnika:

![Diagnostika pomnilnika sistema Windows](media/windows-memory-diagnostic.png)

Ko se računalnik znova zažene, se orodje **za diagnostiko pomnilnika** sistema Windows zažene samodejno. Stanje in napredek bosta prikazana med izvajanjem diagnostike, diagnostiko pa lahko prekličete tako, da pritisnete tipko **ESC** na tipkovnici.

Ko je diagnostika končana, se sistem Windows zažene normalno.
Takoj po ponovnem zagonu, ko se prikaže namizje, se prikaže obvestilo (ob ikoni središča za opravila v opravilni vrstici), ki označuje, ali je prišlo do napak v pomnilniku.  Na primer:

Tukaj je ikona središča za opravila: ![Ikona središča za opravila](media/action-center-icon.png) 

In vzorčno obvestilo: ![Ni napak v pomnilniku](media/no-memory-errors.png)

Če ste izbrali obvestilo,  lahko izberete ikono središče  za opravila v opravilni vrstici, da prikažete središče za opravila in si ogledate seznam obvestil, po ki se jih lahko premikate.

Če si želite ogledati podrobne informacije, **vnesite** dogodek v iskalno polje v opravilni vrstici, nato pa izberite **Pregledovalnik dogodkov.** V levem **podoknu pregledovalnika** dogodkov se pomaknite v okno Dnevniki **> Windows.** V desnem podoknu preglejte seznam, medtem  ko si ogledujete stolpec Vir, dokler ne vidite dogodkov z vrednostjo Source value **MemoryDiagnostics-Results.** Označite vsak tak dogodek in si oglejte informacije o rezultatu v polju pod **zavihkom** Splošno pod seznamom.
