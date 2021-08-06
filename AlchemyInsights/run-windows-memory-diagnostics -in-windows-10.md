---
title: Zagon diagnostike Windows pomnilnika v Windows 10
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
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922587"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Zagon diagnostike Windows pomnilnika v Windows 10

Če Windows in aplikacije v računalniku zrušijo, zamrznejo ali delujejo nestabilen, imate morda težave s pomnilnikom računalnika (RAM). Zaženete lahko orodje Windows pomnilnik, da preverite težave z RAM-om računalnika.

V iskalno polje v opravilni vrstici vnesite **diagnostiko pomnilnika** in nato izberite **Windows Diagnostika pomnilnika.** 

Če želite zagnati diagnostiko, morate računalnik znova zagnati. Na voljo je možnost za takojšni vnovični zagon (shranite svoje delo in najprej zaprite dokumente in e-poštna sporočila) ali pa načrtujte samodejno izvajanje diagnostike ob naslednjem ponovnem zagonu računalnika:

![Windows Diagnostika pomnilnika](media/windows-memory-diagnostic.png)

Ko se računalnik znova zažene, se **Windows orodje za diagnostiko** pomnilnika. Stanje in napredek bosta prikazana med izvajanjem diagnostike, diagnostiko pa lahko prekličete tako, da pritisnete tipko **ESC** na tipkovnici.

Ko je diagnostika končana, se Windows običajno začela.
Takoj po ponovnem zagonu, ko se prikaže namizje, se prikaže obvestilo (ob ikoni središča za opravila v opravilni vrstici), ki označuje, ali je prišlo do napak v pomnilniku.  Na primer:

Tukaj je ikona središča za opravila: ![Ikona središča za opravila](media/action-center-icon.png) 

In vzorčno obvestilo: ![Ni napak v pomnilniku](media/no-memory-errors.png)

Če ste izbrali obvestilo,  lahko izberete ikono središče  za opravila v opravilni vrstici, da prikažete središče za opravila in si ogledate seznam obvestil, po ki se jih lahko premikate.

Če si želite ogledati podrobne informacije, **vnesite** dogodek v iskalno polje v opravilni vrstici, nato pa izberite **Pregledovalnik dogodkov.** V levem **podoknu pregledovalnika** dogodkov se premaknite do Windows **dnevnikov >.** V desnem podoknu preglejte seznam, medtem  ko si ogledujete stolpec Vir, dokler ne vidite dogodkov z vrednostjo Source value **MemoryDiagnostics-Results.** Označite vsak tak dogodek in si oglejte informacije o rezultatu v polju pod **zavihkom** Splošno pod seznamom.
