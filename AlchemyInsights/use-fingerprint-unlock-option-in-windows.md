---
title: Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588331"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10

**Omogoči Windows hello prstni odtis**

Če želite odkleniti sistem Windows 10 s prstnim odtisom, morate nastaviti Windows hello prstni odtis tako, da dodate (dovolite, da se Windows nauči prepoznati) vsaj en prst. 

1. Odprite **možnost nastavitve > računi > možnosti prijave** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)). Navedene bodo razpoložljive možnosti za vpis. Na primer:

    ![Možnosti vpisnega znaka.](media/sign-in-options.png)

2. Kliknite ali tapnite **Windows hello prstni odtis**, nato pa kliknite **Nastavi**. V oknu z nastavitvami sistema Windows hello kliknite **Začni**. Senzor prstnih odtisov bo aktiviran in pozvani boste, da Položite prst na senzor:

   ![Senzor prstnih odtisov.](media/fingerprint-sensor.png)

3. Upoštevajte navodila, ki vas bodo prosila, da večkrat skenirate prst. Ko končate, boste imeli možnost dodajanja drugih prstov, ki jih boste morda želeli uporabiti za vpis. Ko se boste naslednjič prijavili v sistem Windows 10, boste imeli možnost, da to storite s prstnim odtisom.

**Windows hello prstni odtis ni na voljo kot možnost prijave**

Če Windows hello prstni odtis ni prikazan kot možnost v **možnosti prijave**, to pomeni, da Windows ne pozna nobenega bralnika prstnih odtisov/skenerja, priloženega računalniku, ali da sistemska politika preprečuje njegovo uporabo (če na primer vaš računalnik upravlja vaše delovno mesto). Za odpravljanje težav: 

1. V opravilni vrstici izberite gumb **Start** in poiščite **upravitelja naprav**.

2. Kliknite ali tapnite, da odprete **upravitelja naprav**.

3. V upravitelju naprav razširite biometrične naprave tako, da kliknete njegov Chevron.

   ![Biometrične naprave.](media/biometric-devices.png)

4. Optični bralnik prstnih odtisov mora biti naveden kot biometrična naprava, kot je optični bralnik Synaptics WBDI:

   ![Biometrične naprave.](media/biometric-devices-expanded.png)

5. Če optični bralnik prstnih odtisov ni prikazan in je optični bralnik vgrajen v računalnik, obiščite spletno mesto izdelovalca računalnika. V razdelku za tehnično podporo za model računalnika poiščite gonilnik za Windows 10 za skener, ki ga lahko namestite.

6. Če je optični bralnik ločen od računalnika (priložen prek USB-ja), obiščite spletno mesto izdelovalca optičnega bralnika, da poiščete in namestite programsko opremo gonilnika naprave Windows 10 za model optičnega bralnika, ki ga imate.
