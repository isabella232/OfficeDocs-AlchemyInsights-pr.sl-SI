---
title: Profili Intune Wi-Fi
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555814"
---
# <a name="intune-wi-fi-profiles"></a>Profili Intune Wi-Fi

Uspešna izvedba povezljivosti Wi-Fi za odjemalce MDM je odvisna od pravilno uvedenega profila, ki odraža zahteve infrastrukture wi-fi podjetja. Če želite pregledati ustrezne nastavitve za odjemalske platforme, ki jih preiskujete, glejte: 

[Dodajanje nastavitev omrežja Wi-Fi za naprave s sistemom Android v storitvi Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Dodajanje nastavitev wi-fi za namenske in v celoti upravljane naprave za Android Enterprise v storitvi Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Dodajanje nastavitev wi-fi za naprave s sistemom iOS in iPadOS v storitvi Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Dodajanje nastavitev omrežja Wi-Fi za naprave s sistemom Windows 10 in novejšimi napravami v storitvi Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Uvoz nastavitev omrežja Wi-Fi za naprave s sistemom Windows v storitvi Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Pogosta vprašanja**

**Uvajam profil Wi-Fi, ki je odvisen od uvedenega potrdila, določenega v profilu Wi-Fi. Vendar pa konfiguracijski profili prikazujejo stanje napake.**

Preverite, ali je naprava prejela potrdilo.

1. V intunu pojdite na **Vse naprave in** izberite > **napravo**.

2. Preverite, ali so navedeni vsi pričakovani profili in v uspešnem stanju.

3. Če imate za profil androida vmesna potrdila v verigi potrdil, se prepričajte, da so uvedena v napravah Android.

    Če želite preveriti stanje potrdila, pojdite na **Konfiguracija**  >  **naprave Profili**  >  **Posrednik zaupanja vrednega potrdila o pristnosti s sistemom**  >  **Properties**  >  **Android**.

Če še vedno vidite napake, preglejte razdelke s postopki in odpravljanje težav. Če želite več informacij, [glejte Pregled za odpravljanje težav s certifikatnimi profili SCEP z MicrosoftOm Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**V napravo sem poslal profil Wi-Fi. Intune kaže, da je bila uspešna, vendar naprava ne vzpostavlja povezave z omrežjem Wi-Fi.**

Uspešno stanje pomeni, da je Intune uspešno uvedel profil kot konfiguriran. Vendar pa te konfiguracije morda ne ustrezajo vašim zahtevam za omrežje in/ali preverjanje pristnosti. Če želite več podrobnosti o poskusu povezave, preglejte dnevnike v infrastrukturi in storitvi za preverjanje pristnosti (v krmilniku dostopne točke Wi-Fi in strežniku NPS/Radius). Če želite zbirati in pregledovati dnevnike, boste morda morali sodelovati z ekipo za omrežno infrastrukturo ali drugim prodajalcem wi-fi.