---
title: Manjkajoči pogoji iz trgovine SharePoint online Term Store
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053529"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogočanje šifriranja BitLocker z InTune

Za konfiguriranje nastavitev šifriranja Boitlocker za naprave s sistemom Windows, kot je opisano v temi: Windows10 (in novejše) nastavitve za zaščito naprav z InTune, je mogoče uporabiti pravilnik o zaščiti končne točke.

Zavedati se morate, da številne novejše naprave s sistemom Windows 10 podpirajo samodejno šifriranje BitLocker, ki se sproži brez uporabe pravilnika MDM. To lahko vpliva na uporabo pravilnika, če niso konfigurirane privzete nastavitve. Za podrobnejše podrobnosti glejte Pogosta vprašanja.


Pogosta  vprašanja Q: katere izdaje šifriranja naprave s sistemom Windows s pravilnikom o zaščiti končne točke?
 O: nastavitve v pravilniku o zaščiti končne točke se izvajajo s programom BitLocker CSP.BitLocker CSP ne podpira vseh izdaj niti ne gradi sistema Windows. 
      V tem času Windows Editions: Enterprise; Izobraževanje, Mobile, Mobile Enterprise in Professional (od izgradnje 1809 naprej) so podprte.




V: če je naprava že šifrirana s funkcijo BitLocker z uporabo privzetih nastavitev OS za način šifriranja in moč šifre (XTS-AES-128) bo uporabil pravilnik z različnimi nastavitvami samodejno sproži ponovno šifriranje pogona z novimi nastavitvami?

A: ne. Da bi uporabili nove nastavitve šifre, morate pogon najprej dešifrirati.

Opomba za naprave, ki se vpisujejo z avtopilot, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler se ne ovrednoti pravilnik InTune, ki omogoča uporabo nastavitev pravilnika, ki se uporablja namesto privzetih vrednosti OPERACIJSKEGA sistema




Q Če je naprava šifrirana zaradi uporabe pravilnika InTune bo dešifrirati, ko je ta pravilnik odstranjen?

O: odstranitev pravilnika, povezane s šifriranjem, ne povzroči dešifriranje pogonov, ki so bili konfigurirani.




V: zakaj InTune pravilnik o skladnosti kaže, da moja naprava nima "BitLocker Enabled", vendar je?

O: nastavitev» BitLocker Enabled «v pravilniku o izpolnjevanju pravil skladnosti uporablja odjemalca za potrdilo o zdravstvenem stanju naprave Windows (DHA). Ta odjemalec meri samo stanje naprave ob zagonu. Torej, če naprava ni bila znova zagnana, ker je šifriranje BitLocker končano, odjemalska storitev DHA ne bo poročala, da je BitLocker aktiven.