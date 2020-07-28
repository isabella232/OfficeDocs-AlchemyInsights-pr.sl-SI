---
title: Odstranjevanje podatkov in brisanje naprav iz intuna
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440466"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odstranjevanje podatkov in brisanje naprav iz intuna

Dejanja »Upokojijo naprave« in »Device Wipe« lahko odstranite podatke podjetja, ki jih upravlja Intune, ali pa izvedete tovarniško ponastavitev in napravo vrnete na privzete nastavitve.

1. Vpišite se v upravljanje naprav v storitvi Microsoft 365 in odi¹tejejte **aplikacije**  >  **Vse naprave**.
2. Izberite napravo, ki jo želite izbrisati.
3. Izberite vrsto oddaljenega brisa, ki ga želite narediti. Upokojiti izbriše samo organizacijske informacije, medtem ko polni robčki obnovite napravo na tovarniške nastavitve.
4. Izberite **Da,** da potrdite. Dokler se robček ne konča, je stanje dejanja naprave prikazano kot »V teku«.</br>
    Ko je dejanje dokončano, na seznamu upravljane naprave ne boste več videli mobilne naprave.

** Opomba** Podatkov podjetja ni mogoče odstraniti iz naprav, ki so pridružene Azure AD.

Za vse podrobnosti o učinku dejanj »Upokojii« in »Obriši«, vključno s tem, kaj se ohrani in kaj se izbriše, glejte Odstranjevanje naprav [z brisanjem, upokojitvijo ali ročnim odvijanjem naprave](https://docs.microsoft.com/intune/devices-wipe).

Če želite izbrisati vse podatke iz naprave macOS, [glejte Brisanje vseh podatkov iz naprave macOS](https://docs.microsoft.com/intune/device-erase).