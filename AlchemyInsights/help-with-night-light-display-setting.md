---
title: Pomoč pri nastavitvi prikaza nočne svetlobe
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405181"
---
# <a name="help-with-the-night-light-display-setting"></a>Pomoč pri nastavitvi prikaza nočne svetlobe

Če želite izvedeti več o nastavitvah zaslona za nočni čas, [glejte Nastavitev zaslona za nočni čas v sistemu Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)

Če so možnosti nočne svetlobe zatemnjene v nastavitvah, preverite gonilnik zaslona: 

1. Kliknite iskalno polje v opravilni vrstici in **vnesite Upravitelj** naprav ter med **rezultati iskanja** izberite Upravitelj naprav.
1. Razširi **grafične kartice.** 

Žal funkcija nočne svetlobe ni na voljo, če vaša naprava uporablja gonilnik DisplayLink ali osnovni gonilnik grafične kartice.

Funkcija nočne svetlobe uporablja nedavno grafično tehnologijo, zato boste morda morali posodobiti gonilnik grafične kartice:  

- Če želite preveriti, ali so na **voljo** posodobitve, izberite Začni  >    >  **posodobitev nastavitev & Windows**  >  **Update Preveri,** ali so na voljo  >  **posodobitve.**  

OR

- Obiščite spletno mesto podpore izdelovalca strojne opreme, da ročno prenesete in namestite najnovejše gonilnike grafične opreme.

## <a name="reset-night-light-in-the-registry"></a>Ponastavitev nočne svetlobe v registru

Če posodobitev gonilnika grafične kartice ni delovala, boste morda morali ponastaviti nočno svetlobo v registru.  

**Pozor:** Ta korak za odpravljanje težav priporočamo le izkušenim uporabnikom. Če register spremenite nepravilno, lahko pride do resnih težav. Za dodatno varnost pred spreminjanjem registra varnostno kopijo registra, da ga lahko obnovite, če pride do težav.

1. V iskalno polje vnesite **regedit** in med rezultati **iskanja izberite Urejevalnik** registra.

1. Pojdite na ta registrski ključ: 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. Izvozite in izbrišite ta podključ:$$windows.data.bluelightreduction.bluelightreductionstate

1. Izvozite in izbrišite ta podključ:$$windows.data.bluelightreduction.settings

1. Znova zaženite Windows in preverite, ali so na voljo možnosti nočne svetlobe.


