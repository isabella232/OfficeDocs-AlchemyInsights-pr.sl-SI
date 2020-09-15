---
title: Odpravljanje težav z vpisom naprav s sistemom Android v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689970"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Odpravljanje težav z vpisom naprav s sistemom Android v Microsoft InTune

Preglejte spodaj navedene vire, da odpravite težavo zdaj.
  
Nekaj pogostih težav in korakov reševanja:
  
 **Napaka v napravi ni šifrirana v portalu podjetja:** Novejše različice sistema Android, še posebej za začetek z v 7.0, zahtevajo zagonsko kodo, da se prepričate, da je naprava popolnoma šifrirana. Pogoste rešitve so, da omogočite zagonski PIN ali popolnoma šifrirate napravo. Če želite več informacij, preglejte [ta dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 **Naprave se ne morejo sprostiti s storitvijo InTune ali prikazati kot» nezdrava «v konzoli za InTune:** Nekatere naprave Samsung 4,4 in 5,5 se morda ne bodo preverjale v storitvi. V tej težavi so na voljo 3 možne rešitve:
  
1. Ročno odprite program InTune Company portal, ki samodejno sproži sinhronizacijo naprave.

2. Posodobite napravo s sistemom Android 6,0 ali novejšo različico.

3. Onemogočanje programa Samsung Smart Manager za upravljanje portala za InTune. Če želite več podrobnosti o teh težavah in resolucijah, preglejte [ta dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) .

 **Vrsta uporabniških licenc neveljavna** ali pa **uporabniško ime ni prepoznana napaka:** uporabnik mora dodeliti licenco za InTune ali EMS. Preglejte te dokumente, če želite dodeliti licenco prek skrbniškega središča za Office ali portala Azure.
  
Dodatni viri za pomoč pri reševanju težave:
  
1. V [portalu za odpravljanje težav](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) s težavo lahko diagnosticirate in odpravite pogoste napake pri vpisu. Če želite več podrobnosti, preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .

2. Preglejte [ta dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za seznam pogostih napak, ki preprečujejo vpis in resolucije.

3. [Naučite se vpisati naprave s sistemom Android v Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).
