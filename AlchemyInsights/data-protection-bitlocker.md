---
title: DataProtection - Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118610"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Omogočanje šifriranja Bitlocker s funkcijo Intune

S pravilnikom za zaščito končne točke za Intune lahko konfigurirate nastavitve šifriranja Bitlocker za Windows naprave. Če želite več informacij, [Windows 10 (in novejših) nastavitev za zaščito naprav z uporabo storitve Intune.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Poleg pravilnika za zaščito končne točke je na voljo tudi poročilo o šifriranju, ki nudi podrobnejši pogled stanja šifriranja za naprave. Do tega poročila lahko dostopate na portalu MEM v razdelku **Naprave > Monitor** in nato v razdelku **Konfiguracija izberite** Poročilo o [šifriranju.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)

Če ugotovite, da funkcije Bitlocker ni mogoče omogočiti v skladu s pričakovanji ali da je profil, ki se uporablja za omogočanje funkcije Bitlocker, v stanju napake, preglejte poročilo o šifriranju, da boste bolje razumeli, zakaj se pojavlja delovanje.

Če želite podrobnosti o tem, kako interpretirati poročilo, vključno z različnimi vrednostmi stanja šifriranja, glejte [Nadzor šifriranja naprave s intune.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Ne pozabite, da številne novejše naprave s sistemom Windows 10 podpirajo samodejno šifriranje Bitlocker, ki se sproži brez uporabe pravilnika MDM. To lahko vpliva na uporabo pravilnika, če so konfigurirane privzete nastavitve. Več podrobnosti najdete v teh pogostih vprašanjih.

Če želite več informacij o odpravljanju težav s funkcijo bitlocker, [glejte Odpravljanje težav s pravilniki za BitLocker Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**Pogosta vprašanja**

V: Katere izdaje Windows podpirajo šifriranje naprave s pravilnikom za zaščito končne točke?<br>
O: Nastavitve v pravilniku za zaščito končne točke za Intune so posodobljene z uporabo storitve [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). Vse izdaje ali Windows ne podpirajo storitve Bitlocker CSP. <br><br>

V: Kako je mogoče Bitlocker omogočiti v napravah, ne da bi potrebovali interakcijo s končnim uporabnikom?<br>
O: Če so izpolnjeni zahtevani predpogoji, lahko s funkcijo Bitlocker »Tiho šifriranje« omogočite prek storitve Intune. Oglejte si podrobnosti zahtev naprave in vzorčne nastavitve pravilnika za omogočanje tihega šifriranja v tem dokumentu: [Tiho omogočanje šifriranja bitlocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices). <br><br>

V: Če je naprava že šifrirana s funkcijo Bitlocker s privzetimi nastavitvami operacijskega sistema za način šifriranja in moč cipher (XTS-AES-128), bo program uporabil pravilnik z različnimi nastavitvami, ki samodejno sproži ponovno šifriranje pogona z novimi nastavitvami?<br>
O: Ne. Če želite uporabiti nove nastavitve cipher, morate najprej dešifrirati pogon.<br><br>
**Opomba:** Za naprave, ki so včlanjene s funkcijo Autopilot, se samodejno šifriranje, ki bi se pojavilo med OOBE, ne sproži, dokler ni ovrednoten pravilnik za Intune, kar omogoča uporabo nastavitev na podlagi pravilnika na mestu privzetih nastavitev operacijskega sistema.
 
V: Ali bo naprava šifrirana zaradi uporabe pravilnika za Intune, ali bo dešifrirana, ko bo ta pravilnik odstranjen?<br>
O: Odstranjevanje pravilnika, ki je povezan s šifriranjem, NE povzroči dešifriranja pogonov, ki so bili konfigurirani.
 
V: Zakaj pravilnik o skladnosti s predpisi za Intune kaže, da v moji napravi ni omogočena storitev Bitlocker, čeprav je?<br>
O: Nastavitev »Bitlocker je omogočena« v pravilniku o skladnosti s predpisi storitve Intune uporablja odjemalca Windows potrditev ustreznosti stanja naprave (DHA). Ta odjemalec meri le stanje naprave v času zagona. Če torej naprava ni bila znova zagnala, odkar je bilo šifriranje Bitlocker dokončano, storitev odjemalca DHA ne bo prijavila funkcije Bitlocker kot aktivna.
 
 