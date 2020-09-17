---
title: Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795260"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>Uporaba možnosti odklepanja prstnih odtisov v sistemu Windows 10

**Omogočanje pozdravnega prstnega odtisa sistema Windows**

Če želite odkleniti Windows 10 s prstnim odtisom, morate nastaviti pozdravni prstni odtis sistema Windows, tako da dodate (oddajanje sistema Windows se naučite prepoznati) vsaj en prst. 

1. Pojdite na **nastavitve > računov > možnosti za vpis** (ali kliknite [tukaj](ms-settings:signinoptions?activationSource=GetHelp)). Na voljo bodo navedene možnosti za vpis. Na primer:

    ![Možnosti vpisa.](media/sign-in-options.png)

2. Kliknite ali tapnite **Pozdravni prstni odtis sistema Windows**, nato pa kliknite **Nastavi**. V oknu Windows hello **setup kliknite Začni**. Senzor prstnih odtisov bo aktiviran in pozvani boste, da postavite kazalec na tipalo:

   ![Senzor prstnih odtisov.](media/fingerprint-sensor.png)

3. Sledite navodilom, ki vas bodo pozvali, da večkrat skenirate prst. Ko je ta možnost končana, boste lahko dodali še druge prste, ki jih boste morda želeli uporabiti za vpis. Ko se naslednjič vpišete v sistem Windows 10, boste imeli na voljo možnost uporabe prstnega odtisa.

**Pozdravni prstni odtis sistema Windows ni na voljo kot možnost za vpis**

Če se prstni odtis sistema Windows ne prikaže kot možnost v **možnostih za vpis**, to pomeni, da Windows ne pozna nobenega bralnika prstnih odtisov ali skenerja, ki je priključen na vaš računalnik, ali da sistemska politika preprečuje njegovo uporabo (če je na primer vaš računalnik upravljan na delovnem mestu). Odpravljanje težav: 

1. V opravilni vrstici izberite gumb **Start** in poiščite **upravitelja naprav**.

2. Kliknite ali tapnite, da odprete **upravitelja naprav**.

3. V upravitelju naprav razširite biometrične naprave tako, da kliknete njen Chevron.

   ![Biometrične naprave.](media/biometric-devices.png)

4. Bralnik prstnih odtisov bi moral biti naveden kot biometrična naprava, kot je na primer Synaptics WBDI Scanner:

   ![Biometrične naprave.](media/biometric-devices-expanded.png)

5. Če skenerja prstnih odtisov ni prikazan in je optični bralnik vdelan v računalnik, obiščite spletno mesto izdelovalca računalnika. V razdelku tehnična podpora za model računalnika poiščite gonilnik sistema Windows 10 za skener, ki ga lahko namestite.

6. Če je optični bralnik ločen od računalnika (priloženo prek USB-ja), obiščite spletno mesto izdelovalca optičnega bralnika, da poiščete in namestite programsko opremo gonilnika naprave Windows 10 za model skenerja, ki ga imate.
