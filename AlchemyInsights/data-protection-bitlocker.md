---
title: Zaščita podatkov-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908725"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogočanje šifriranja BitLocker z InTune

 Za konfiguriranje nastavitev šifriranja BitLocker za naprave s sistemom Windows lahko uporabite pravilnik o zaščiti končne točke. Če želite več informacij, glejte [nastavitve sistema Windows 10 (in novejše) za zaščito naprav z InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
Zavedati se morate, da številne novejše naprave s sistemom Windows 10 podpirajo samodejno šifriranje BitLocker, ki se sproži brez uporabe pravilnika MDM. To lahko vpliva na uporabo pravilnika, če so konfigurirane neprivzete nastavitve. Za podrobnejše podrobnosti si oglejte ta pogosta vprašanja.
 
Če želite več informacij o odpravljanju težav s funkcijo BitLocker, glejte [Odpravljanje težav s pravilniki funkcije BitLocker v programu Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Faq**

 V: katere izdaje šifriranja naprave sistema Windows z uporabo pravilnika o zaščiti končnih točk?<br>
 O: nastavitve v pravilniku o zaščiti končne točke se izvajajo s programom [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Program BitLocker CSP ne podpira vseh izdaj ali nadgradi sistema Windows. <br><br>
      V tem času so podprte naslednje izdaje sistema Windows: Enterprise, Education, Mobile, Mobile Enterprise in Professional (gradnja 1809 in novejše različice).
 
V: če je naprava že šifrirana s funkcijo BitLocker z uporabo privzetih nastavitev OS za način šifriranja in moč šifre (XTS-AES-128), bo uporaba pravilnika z različnimi nastavitvami samodejno sprožila ponovno šifriranje pogona z novimi nastavitvami?<br>
A: ne. Če želite uporabiti nove nastavitve šifre, morate najprej dešifrirati pogon.<br><br>
**Opomba:** Za naprave, ki se vpisujejo z avtopilot, se samodejno šifriranje, ki se pojavi med OOBE, ne sproži, dokler se ne ovrednoti pravilnik InTune, ki omogoča uporabo nastavitev pravilnika, ki se uporablja namesto privzetih vrednosti OPERACIJSKEGA sistema.
 
V: če je naprava šifrirana zaradi uporabe pravilnika InTune, ali bo dešifrirala, ko je ta pravilnik odstranjen?<br>
O: odstranitev pravilnika, povezane s šifriranjem, ne povzroči dešifriranja pogonov, ki so bili konfigurirani.
 
V: zakaj InTune pravilnik o skladnosti kaže, da moja naprava nima omogočenega pogona BitLocker, čeprav je?<br>
O: nastavitev» BitLocker Enabled «v pravilniku o skladnosti s skladnostjo uporablja odjemalca za potrdilo o zdravstvenem stanju naprave Windows (DHA). Ta odjemalec meri samo stanje naprave ob zagonu. Če naprava ni bila znova zagnana, ker je šifriranje BitLocker končano, odjemalska storitev DHA ne bo poročala, da je BitLocker aktiven.
 
 