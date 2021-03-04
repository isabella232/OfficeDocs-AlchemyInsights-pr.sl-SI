---
title: Odstranjevanje podatkov in počistite napravo iz Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416329"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Odstranjevanje podatkov in počistite napravo iz Intune

Oddaljena dejanja Ukinitev naprave in Brisanje podatkov iz naprave lahko uporabite za odstranitev podatkov podjetja, ki jih upravlja Intune, ali za ponastavitev na tovarniške nastavitve in vrnitev naprave na privzete nastavitve.

1. Prijavite se v Upravljanje naprav okolja Microsoft 365 in pojdite na **Naprave** > **Vse naprave**.
2. Izberite napravo, ki jo želite počistiti.
3. Izberite vrsto oddaljenega brisanja, ki ga želite izvesti. Ukinitev izbriše samo organizacijske podatke, popolno brisanje podatkov iz naprave pa obnovi tovarniške nastavitve naprave.
4. Za potrditev kliknite **Da**. Dokler se brisanje ne konča, se stanje dejanja naprave prikazuje kot *Ukinitev v čakanju*.
    Po končanem dejanju mobilna naprava ne bo več vidna na seznamu upravljane naprave.

> [!NOTE]
> Podatkov podjetja ni mogoče odstraniti iz naprav, PRIDRUŽENIH Azure AD. 

Za vse podrobnosti o učinku ukrepov ukinitve in brisanja, vključno s tem, kaj se obdrži in kaj izbriše, glejte naslednjo dokumentacijo:

- [Odstranite naprave z brisanjem, ukinitvijo ali ročnim odjavljanjem naprave](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).
- [Kako izbrisati samo poslovne podatke iz aplikacij, ki jih upravlja Intune](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [Izbrišite vse podatke iz naprave macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).