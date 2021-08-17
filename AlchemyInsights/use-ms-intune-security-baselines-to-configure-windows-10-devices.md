---
title: Uporaba Microsoft Intune varnostnih osnovnih načrta za konfiguracijo Windows 10 naprave
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104360"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Uporaba Microsoft Intune varnostnih osnovnih načrta za konfiguracijo Windows 10 naprave

Osnovni osnovni osnovni stroški varnosti za Intune ščitijo uporabnike in naprave. Varnostni osnovni osnovni Windows vnaprej konfigurirane skupine, ki se uporabljajo za uporabo znane skupine nastavitev in privzetih vrednosti, ki jih priporočajo ustrezne varnostne skupine. Z ustvarjanjem profila varnostnega osnovnega načrta v programu Intune ustvarite predlogo, ki je sestavljena iz več profilov za konfiguracijo naprave.

Ko uvedete varnostne osnovne vrstice za skupine uporabnikov ali naprav, so nastavitve uporabljene za naprave, ki se izvajajo v Windows 10 ali novejših različicah. Na primer, MDM Security Baseline samodejno (1) omogoči BitLocker za izmenljive pogone, (2) zahteva geslo za odklepanje naprave in (3) onemogoči osnovno preverjanje pristnosti. Če privzeta vrednost ne deluje v vašem okolju, prilagodite osnovni načrt tako, da bo veljal za vse nastavitve, ki jih potrebujete.

Z varnostnimi osnovnimi črtami lahko tudi vzpostavite varen potek dela v Microsoft 365. Spodaj so nekatere prednosti tega:

- Osnovni načrt varnosti vključuje najboljše prakse in priporočila za nastavitve, ki vplivajo na varnost. Ker intune v sodelovanju z varnostno Windows, ki ustvari osnovne vrstice za pravilnike skupine, ta priporočila temeljijo na obseženih navodilih in obsežni izkušnji.
- Če še ne veste, kje začeti Intune, potem vam bodo varnostni osnovni načrti pomagali hitro ustvariti in uvesti varni profil.
- Če trenutno uporabljate pravilnik skupine, je selitev v Intune za namene upravljanja veliko preprostejša z varnostnimi osnovnimi črtami, ker so vgrajeni v Intune in vključujejo vrhunskih zmogljivosti za upravljanje.

Če želite več informacij, [Windows varnostne osnovne vrstice](https://go.microsoft.com/fwlink/?linkid=2141503) [in Upravljanje mobilnih naprav.](https://go.microsoft.com/fwlink/?linkid=2141701)