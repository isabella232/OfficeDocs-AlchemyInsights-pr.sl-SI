---
title: Uporabite osnovne varnostne črte Microsoft InTune, da konfigurirate naprave s sistemom Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696382"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Uporaba osnovnih varnostnih črt za Microsoft InTune za konfiguriranje naprav s sistemom Windows 10

InTune varnostne osnovne črte omogočajo zaščito uporabnikov in naprav. Osnovne varnostne črte so nastavitve sistema Windows, ki so bile vnaprej konfigurirane za uporabo znane skupine nastavitev in privzetih vrednosti, ki jih priporoča ustrezna varnostna ekipa. Z ustvarjanjem profila varnostnega osnovnega načrta v programu InTune ustvarite predlogo, ki je sestavljena iz več profilov za konfiguracijo naprav.

Ko uvedete varnostne osnovne črte v skupine uporabnikov ali naprav, so nastavitve uporabljene v napravah, ki se izvajajo v sistemu Windows 10 ali novejših različicah. Na primer, če se samodejno varnostno izhodišče Microsoft Mobile Device Management (MDM) (1) omogoči BitLocker za izmenljive pogone, (2) zahteva geslo za sprostitev naprave in (3) onemogoči osnovno preverjanje pristnosti. Ko privzeta vrednost ne deluje v vašem okolju, lahko prilagodite osnovni načrt, da uporabite nastavitve, ki jih potrebujete.

Varnostne osnovne črte omogočajo tudi vzpostavitev varnega poteka dela od konca do konca v programu Microsoft 365. Spodaj so navedene nekatere prednosti te funkcije:
- V osnovnem načrtu varnosti so na voljo najboljše prakse in priporočila za nastavitve, ki vplivajo na varnost. Ker InTune partnerji z varnostno skupino sistema Windows, ki ustvari osnovne predloge za pravilnike skupine, ta priporočila temeljijo na trdnih navodilih in obširnih izkušnjah.
- Če ste šele začeli uporabljati InTune in ne veste, kje začeti, vam bodo varnostne osnovne črte pomagale hitro ustvariti in uvesti varen profil.
- Če trenutno uporabljate pravilnik skupine, je selitev v program za upravljanje precej lažja, saj so te osnovne varnostne črte vgrajene v InTune in vključujejo vrhunske zmogljivosti za upravljanje.

Če želite več informacij, glejte [osnovne varnostne črte sistema Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) in [upravljanje mobilnih naprav](https://docs.microsoft.com/windows/client-management/mdm/).