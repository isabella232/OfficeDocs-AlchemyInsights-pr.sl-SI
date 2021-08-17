---
title: Uporaba Microsoft Intune varnostnih osnovnih načrta za konfiguracijo Windows 10 naprave
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886648"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Uporaba Microsoft Intune varnostnih osnovnih načrta za konfiguracijo Windows 10 naprave

Osnovni osnovni osnovni stroški varnosti za Intune ščitijo uporabnike in naprave. Varnostni osnovni osnovni Windows vnaprej konfigurirane skupine, ki se uporabljajo za uporabo znane skupine nastavitev in privzetih vrednosti, ki jih priporočajo ustrezne varnostne skupine. Z ustvarjanjem profila varnostnega osnovnega načrta v intune ustvarite predlogo, ki je sestavljena iz več profilov za konfiguracijo naprave.

Ko uvedete varnostne osnovne vrstice za skupine uporabnikov ali naprav, so nastavitve uporabljene za naprave, ki se izvajajo v Windows 10 ali novejšem. Na primer, varnostna osnovna črta upravljanja Microsoftovih mobilnih naprav (MDM) samodejno omogoči BitLocker za izmenljive pogone, zahteva geslo za odklepanje naprave in onemogoči osnovno preverjanje pristnosti. Če privzeta vrednost ne deluje v vašem okolju, lahko prilagodite osnovni načrt tako, da uporabi nastavitve, ki jih potrebujete.

Z varnostnimi osnovnimi črtami lahko tudi vzpostavite varen potek dela v Microsoft 365. Osnovni načrt varnosti vključuje najboljše prakse in priporočila za nastavitve, ki vplivajo na varnost. Intune v sodelovanju z varnostno skupino za Windows, ki ustvari osnovne vrstice za pravilnike skupine, zato ta priporočila temeljijo na zanesljivih navodilih in obsežni izkušnji.

Če še ne veste, kje začeti Intune, in ne veste, kje začeti, vam varnostni osnovni načrt pomaga hitro ustvariti in uvesti varen profil. Če trenutno uporabljate pravilnik skupine, je selitev v Intune za namene upravljanja veliko preprostejša z varnostnimi osnovnimi črtami, ker so vgrajeni v Intune in vključujejo vrhunske zmogljivosti upravljanja.

Če želite izvedeti več, [glejte Windows varnostni osnovni načrt in](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) Upravljanje [mobilnih naprav.](https://docs.microsoft.com/windows/client-management/mdm/)

