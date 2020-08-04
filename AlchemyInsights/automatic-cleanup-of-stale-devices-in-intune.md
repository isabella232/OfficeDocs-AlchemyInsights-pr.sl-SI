---
title: Samodejno čiščenje zastarelih naprav v intunu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555734"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Samodejno čiščenje zastarelih naprav v intunu

Intune omogoča admin nastaviti časovni interval med 90 in 270 dni, po katerem zastarele naprave so odstranjene iz storitve. Ta nastavitev je organizacija na stežaj in ko je aktivirana začne veljati takoj. Vse naprave, ki niso bile prijavljene v strežnik Intune za obdobje, ki presega nastavitev, se trajno izbrišejo.

** Opomba** Za to čiščenje so primerni samo predmeti naprave MDM. Izključeni so samo predmeti naprave EAS.

Za dodatne informacije o tem, kdaj naprava postane primerna za izbris na podlagi nastavitve čiščenja naprave in njenega "stanja":

Nastavitev: **Brisanje naprav po zadnjem datumu prijave: Da (določena vrednost (N) v določenih dneh)**

- Na podlagi vrednosti (N), konfigurirane v nastavitvi, storitev Intune izbriše napravo v določenih dneh po tem, ko se je nazadnje uspešno všli.

Nastavitev: **Brisanje naprav po zadnjem datumu prijave: Ne**

- 180 dni po izteku veljavnosti potrdila o napravi in se ne obnovi, se naprava izbriše.

** Opomba** V obeh primerih mora biti naprava uspešno registrirana v intunu. Registracija se zgodi med prvim preverjanjem naprave s storitvijo Intune.

Če se naprava uspešno vpiše v intune, vendar ne registrira intune, se naprava izbriše 270 dni po vpisu. (90 dni, da označite napravo kot preklicano, nato pa še 180 dni za brisanje zapisa.)

Trenutno v konzoli Intune trenutno ni mehanizma za določitev datuma poteka certifikata naprave za katero koli napravo.