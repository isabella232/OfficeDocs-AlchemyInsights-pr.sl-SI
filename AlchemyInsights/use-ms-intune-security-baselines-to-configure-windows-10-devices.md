---
title: Uporabite Microsoft InTune varnostne osnovne črte, da konfigurirate naprave s sistemom Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573788"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Uporabite Microsoft InTune varnostne osnovne črte, da konfigurirate naprave s sistemom Windows 10

InTune varnostne osnovne črte omogočajo zaščito uporabnikov in naprav. Osnovne varnostne črte so nastavitve sistema Windows, ki so bile vnaprej konfigurirane za uporabo znane skupine nastavitev in privzetih vrednosti, ki jih priporoča ustrezna varnostna ekipa. Z ustvarjanjem profila varnostnega osnovnega načrta v programu InTune ustvarite predlogo, ki je sestavljena iz več profilov za konfiguracijo naprav.

Ko uvedete varnostne osnovne črte v skupine uporabnikov ali naprav, so nastavitve uporabljene v napravah, ki se izvajajo v sistemu Windows 10 ali novejši različici. Na primer, MDM Security Basicove vrstice samodejno (1) omogoči BitLocker za izmenljive pogone, (2) zahteva geslo za sprostitev naprave in (3) onemogoči osnovno preverjanje pristnosti. Ko privzeta vrednost ne deluje v vašem okolju, prilagodite osnovni načrt, da uporabite nastavitve, ki jih potrebujete.

Varnostne osnovne črte omogočajo tudi vzpostavitev varnega poteka dela od konca do konca v programu Microsoft 365. Spodaj so navedene nekatere prednosti:

- V osnovnem načrtu varnosti so na voljo najboljše prakse in priporočila za nastavitve, ki vplivajo na varnost. Ker InTune partnerji z varnostno skupino sistema Windows, ki ustvari osnovne predloge za pravilnike skupine, ta priporočila temeljijo na trdnih navodilih in obširnih izkušnjah.
- Če ste šele začeli uporabljati InTune in ne veste, kje začeti, vam bodo varnostne osnovne črte pomagale hitro ustvariti in uvesti varen profil.
- Če trenutno uporabljate pravilnik skupine, je selitev v InTune za upravljanje precej lažja z osnovnimi varnostnimi črtami, ker so vgrajene v InTune in vključujejo vrhunske zmogljivosti za upravljanje.

Če želite izvedeti več, glejte [osnovne varnostne črte sistema Windows](https://go.microsoft.com/fwlink/?linkid=2141503) in [upravljanje mobilnih naprav](https://go.microsoft.com/fwlink/?linkid=2141701).