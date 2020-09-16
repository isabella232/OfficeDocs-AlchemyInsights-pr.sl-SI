---
title: DataProtection – BitLocker
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
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731255"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogočanje šifriranja BitLockerja s funkcijo InTune

 Če želite konfigurirati nastavitve šifriranja BitLockerja za naprave s sistemom Windows, lahko nastavite pravilnik o zaščiti končnih točk. Če želite več informacij, glejte [nastavitve sistema Windows 10 (in novejše različice) za zaščito naprav s funkcijo InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Zavedati se morate, da številne novejše naprave, v katerih je nameščen Windows 10, podpirajo samodejno šifriranje BitLockerja, ki se sproži brez uporabe pravilnika MDM. To lahko vpliva na uporabo pravilnika, če so konfigurirane privzete nastavitve. Če želite več podrobnosti, si oglejte ta pogosta vprašanja.
 
Če želite več informacij o odpravljanju težav z BitLockerjem, glejte [Odpravljanje težav s pravilniki BitLockerja v programu Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Pogosta vprašanja**

 V: katere izdaje šifriranja naprave s sistemom Windows s pravilnikom o zaščiti končnih točk?<br>
 A: nastavitve v pravilniku o zaščiti končnih točk se izvajajo s sistemom [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Niso vse izdaje ali gradi sistema Windows, ki podpirajo sistem BitLocker. <br><br>
      V tem trenutku so podprte te izdaje sistema Windows: Enterprise, Education, Mobile, Mobile Enterprise in Professional (graditev 1809 in novejša različica).
 
V: če je naprava že šifrirana s funkcijo BitLocker s privzetimi nastavitvami sistema OS za način šifriranja in trdnost ključa (XTS-AES-128), bo uporaba pravilnika z različnimi nastavitvami samodejno sprožil vnovično šifriranje pogona z novimi nastavitvami?<br>
O: Ne. Če želite uporabiti nove nastavitve šifer, mora biti pogon najprej dešifriran.<br><br>
**Opomba:** Za naprave, ki so vpisane s samodejnim pilotom, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler ni ovrednoten pravilnik, ki omogoča uporabo nastavitev pravilnika, ki jih je treba uporabiti namesto privzetih vrednosti za OS.
 
V: če je naprava šifrirana zaradi uporabe pravilnika za InTune, bo dešifrirana, ko je ta pravilnik odstranjen?<br>
A: odstranitev pravilnika, povezanega s šifriranjem, ne povzroči dešifriranja pogonov, ki so bili konfigurirani.
 
V: zakaj pravilnik o skladnosti s predpisi pokaže, da moja naprava nima omogočenega pogona BitLocker, čeprav je?<br>
A: nastavitev» BitLocker Enabled «v pravilniku o skladnosti s predpisi uporablja odjemalca za potrdilo o zdravstvenem stanju sistema Windows (DHA). Ta odjemalec samo določi stanje naprave ob zagonu. Če naprava ni bila znova zagnana, ker je bila šifrirana BitLocker dokončana, odjemalska storitev DHA ne bo prijavila funkcije BitLocker kot aktivno.
 
 