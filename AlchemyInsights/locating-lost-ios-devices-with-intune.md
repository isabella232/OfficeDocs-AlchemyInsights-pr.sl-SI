---
title: Iskanje izgubljenih naprav s sistemom iOS z napravo Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440429"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Iskanje izgubljenih naprav s sistemom iOS z napravo Intune

Če omogočite izgubljeni način v napravi s sistema iOS, lahko skrbnik na zaklenjenem zaslonu prikaže sporočilo in telefonsko številko stika.

Ko je omogočen izgubljeni način, lahko skrbnik uporabi dejanje Iskanje naprave za prepoznavanje fizične lokacije naprave.

Dejanje najdi napravo v intunu deluje z napravami s sistemom iOS, da prikaže lokacijo določene naprave na zemljevidu.

Če uporabite to dejanje, mora biti naprava s sistemom iOS v:

- Nadzorovani način
- Izgubljeni način

Če želite več informacij, [glejte Omogočanje izgubljenega načina v napravah s sistemom iOS/iPadOS z napravama Intune in Poiščite izgubljene](https://docs.microsoft.com/intune/device-lost-mode) [ali ukradene naprave iOS/iPadOS z napravami Intune](https://docs.microsoft.com/intune/device-locate).

**Pogosta vprašanja**

V: Izdal sem oddaljeno dejanje za odstranitev podatkov podjetja iz naprave, zdaj pa je obtičal v stanju čakanja.

O: Če želite, da se oddaljeno dejanje uspešno dokonča, mora biti ciljna naprava dosegljiva in zdrava. V teh primerih oddaljeno dejanje ostane v stanju čakanja 30 dni ali dokler naprava ne potrdi ukaza:

- Če naprava nima povezave
- Ko naprava izgubi status upravljanja z napravo Intune

Če menite, da se naprava ne bo več prijavila in da ne bo mogla odstraniti podatkov podjetja, izberite Izbriši. Če izbrišete napravo, odstranite zapis naprave, tako da ga ne bo več na seznamu naprav Intune. Če naprava znova postane aktivna, jo bo moral uporabnik znova včlatiti.

V: Zakaj nekatera oddaljena dejanja niso na voljo za uporabo?

O: Vse platforme ne podpirajo vseh dejanj oddaljenih naprav. Naslednja oddaljena dejanja so specifična za platformo, zato so na voljo samo za ugotovljene platforme.

- Bypass Activation Lock (samo za iOS)
- Nov začetek (samo windows)
- Izgubljen način (samo za iOS)
- Iskanje naprave (samo za iOS)
- Vnovični zagon (samo windows)

Če želite več podrobnosti o vsakem dejanju, glejte Dejanja [naprave, ki so na voljo](https://docs.microsoft.com/intune/device-management#available-device-actions).