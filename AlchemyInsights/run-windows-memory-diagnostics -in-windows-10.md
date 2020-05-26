---
title: Zaženite Windows Memory diagnostika v operacijskem sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358294"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Zaženite Windows Memory diagnostika v operacijskem sistemu Windows 10

Če se Windows in aplikacije v računalniku zrušijo, zamrzujejo ali delujejo na nestabilen način, imate morda težave s pomnilnikom računalnika (RAM-a). Če želite preveriti težave z RAM-om računalnika, lahko zaženete diagnostiko pomnilnika sistema Windows.

V iskalno polje v opravilni vrstici vnesite **diagnostično pomnilniško kartico**in nato izberite **diagnostično pomnilniško kartico Windows**. 

Če želite zagnati diagnostiko, se mora računalnik znova zagnati. Vi življati predkupna pravica v zopet začeti takoj (prosim zaščititi vaš opus ter blizu plan listina ter črka e-verižna srajca prvi), ali tabela spoznati bolezen teči automatically naslednji čas PC zopet začeti:

![Diagnostika pomnilnika sistema Windows](media/windows-memory-diagnostic.png)

Ko se računalnik znova zažene, se bo **orodje za diagnostiko pomnilnika sistema Windows** samodejno zagnali. Stanje in napredek bosta prikazana kot diagnostična vaja, vi pa imate možnost preklica diagnostike tako, da na tipkovnici udarjajte tipko **ESC** .

Ko je diagnostika končana, se Windows zažene normalno.
Takoj po vnovičnem zagonu, ko se prikaže namizje, se prikaže obvestilo (poleg ikone **središča za opravila** v opravilni vrstici), da označite, ali so bile najdene napake v pomnilniku. Na primer:

Tukaj je ikona središča za opravila: ![Ikona središča za opravila](media/action-center-icon.png) 

In vzorčno obvestilo: ![Brez pomnilniških napak](media/no-memory-errors.png)

Če ste obvestilo zamudili, lahko v opravilni vrstici izberete ikono **središče za opravila** , da prikažete središče za **opravila** in si ogledate seznam obvestil, ki jih je mogoče zapisati.

Če želite pregledati podrobne informacije, v iskalno polje v opravilni vrstici vnesite **dogodek** in nato izberite **Pregledovalnik dogodkov**. V levem podoknu **pregledovalnika dogodkov**krmarite do **dnevnikov sistema Windows > System**. V desnem podoknu skenirajte seznam med iskanjem v **izvornem** stolpcu, dokler ne vidite dogodkov z izvorno vrednostjo **memorydiagnostics-rezultati**. Označite vsak tak dogodek in si oglejte informacije o rezultatih v polju pod zavihkom **splošno** pod seznamom.
