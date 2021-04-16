---
title: Možnost odklepanja prstnih odtisov v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796693"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Možnost odklepanja prstnih odtisov v sistemu Windows 10

**Omogočanje prstnih odtisov s funkcijo Windows Hello**

Če želite odkleniti sistem Windows 10 s prstnim odtisom, morate nastaviti prstni odtis Windows Hello tako, da dodate vsaj en prst (tako da sistem Windows prepozna). 

1. Pojdite na **Nastavitve > Računi > možnosti vpisa** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)). Na seznamu bodo navedene razpoložljive možnosti za vpis. Na primer:

    ![Možnosti vpisa.](media/sign-in-options.png)

2. Kliknite ali tapnite **Windows Hello prstni** odtis , nato pa kliknite **Nastavitev**. V oknu za namestitev Windows Hello kliknite **Uvod.** Senzor prstnih odtisov se bo aktiviral in pozvani boste, da postavite prst na senzor:

   ![Senzor prstnih odtisov.](media/fingerprint-sensor.png)

3. Upoštevajte navodila, ki vas bodo pozvala, da večkrat pregledate prst. Ko bo ta rešitev končana, lahko dodate druge prste, ki jih boste morda želeli uporabiti za vpis. Ko se boste naslednjič vpisati v Windows 10, boste imeli možnost, da za to uporabite svoj prstni odtis.

**Možnost za vpis s prstnim odtisom Windows Hello ni na voljo**

Če možnost Prstni odtis Windows Hello ni prikazana kot možnost v možnostih vpisa, sistem Windows ne pozna bralnika prstnih odtisov/optičnega bralnika, ki je priključen na računalnik, ali da sistemski pravilnik preprečuje njegovo uporabo (če na primer vaš računalnik upravlja vaše delovno mesto). Odpravljanje težav: 

1. Izberite gumb **za začetni** meni v opravilni vrstici in poiščite **Upravitelja naprav**.

2. Kliknite ali tapnite, da odprete **upravitelja naprav.**

3. V upravitelju naprav razširite biometrične naprave tako, da kliknete škarne.

   ![Biometrične naprave.](media/biometric-devices.png)

4. Optični bralnik za prstni odtis mora biti naveden kot biometrična naprava, kot je optični bralnik Synaptics WBDI:

   ![Biometrične naprave.](media/biometric-devices-expanded.png)

5. Če bralnik prstnih odtisov ni prikazan in je optični bralnik integriran z vašim računalnikom, obiščite spletno mesto izdelovalca računalnika. V razdelku za tehnično podporo za svoj model računalnika poiščite gonilnik sistema Windows 10, da poiščete optični bralnik, ki ga lahko namestite.

6. Če je optični bralnik ločen od računalnika (priključen prek USB-ja), obiščite spletno mesto izdelovalca optičnega bralnika in poiščite ter namestite programsko opremo gonilnika naprave s sistemom Windows 10 za model optičnega bralnika, ki ga imate.
