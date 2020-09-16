---
title: Pogoji, ki jih ni v trgovini SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750467"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogočanje šifriranja BitLockerja s funkcijo InTune

Če želite konfigurirati nastavitve šifriranja Boitlocker za naprave s sistemom Windows, kot je opisano v: Windows10 (in novejših), uporabite nastavitve za zaščito naprav s funkcijo InTune

Zavedati se morate, da številne novejše naprave, v katerih je nameščen Windows 10, podpirajo samodejno šifriranje BitLockerja, ki se sproži brez uporabe pravilnika MDM. To lahko vpliva na uporabo pravilnika, če niso privzete nastavitve konfigurirane. Če želite več podrobnosti, glejte Pogosta vprašanja.


Pogosta vprašanja   o tem: katere izdaje šifriranja naprave za Windows podpirajo s pravilnikom o zaščiti končnih točk?
 A: nastavitve v pravilniku o zaščiti končnih točk se izvajajo s sistemom BitLocker CSP.Ni vseh izdaj in ne gradi sistema Windows, ki podpirajo sistem BitLocker. 
      V tem času izdaje sistema Windows: Enterprise; Podpora za izobraževanje, mobilno, mobilno podjetništvo in Professional (od gradnje 1809 naprej).




V: če je naprava že šifrirana s funkcijo BitLocker s privzetimi nastavitvami sistema OS za način šifriranja in trdnost ključa (XTS-AES-128), bo uporaba pravilnika z različnimi nastavitvami samodejno sprožil vnovično šifriranje pogona z novimi nastavitvami?

O: Ne. Če želite uporabiti nove nastavitve šifer, mora biti pogon najprej dešifriran.

Opomba pri napravah, ki so vpisani s samodejnim avtopilotom, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler ni ovrednoten pravilnik, ki omogoča uporabo nastavitev pravilnika, ki jih je treba uporabiti namesto privzetih vrednosti za OS.




Q Če je naprava šifrirana zaradi uporabe pravilnika za InTune, bo dešifrirana, ko je ta pravilnik odstranjen?

A: odstranitev pravilnika, povezanega s šifriranjem, ne povzroči dešifriranja pogonov, ki so bili konfigurirani.




V: zakaj pravilnik o skladnosti s predpisi pokaže, da moja naprava nima omogočene funkcije» BitLocker «;

A: nastavitev» BitLocker Enabled «v pravilniku o skladnosti s predpisi, ki uporablja odjemalca s sistemom Windows za zdravstveno varstvo (DHA). Ta odjemalec samo določi stanje naprave ob zagonu. Če naprava ni bila znova zagnana, ker je bilo šifriranje BitLocker dokončano, odjemalska storitev DHA ne bo prijavila funkcije BitLocker kot aktivno.