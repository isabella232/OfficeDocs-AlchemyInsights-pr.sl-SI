---
title: Odpravljanje težav z včlanjanjem naprav Android v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759636"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Odpravljanje težav z včlanjanjem naprav Android v Microsoft InTune

Preglejte spodaj navedene vire, da odpravite težavo zdaj.
  
Nekatera pogosta vprašanja in koraki reševanja:
  
 **Naprava ni šifrirana napaka v portalu podjetja:** Novejše različice Androida, zlasti začenši z v 7.0, zahtevajo geslo za zagon, da zagotovite, da je naprava popolnoma šifrirana. Pogoste rešitve omogočajo zagonsko kodo ali popolnoma šifriranje naprave. Če želite več informacij, preglejte [ta dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 **Naprave ne da se preveri v s storitvijo InTune ali izpis kot "nezdrava" v InTune admin konzolo:** Nekateri Samsung 4,4 in 5,5 naprave morda ne bodo preverili v storitvi. Obstaja 3 možne rešitve za to vprašanje:
  
1. Ročno odprite program InTune Company portal, ki bo samodejno inicializiral sinhronizacijo naprave.

2. Posodobite napravo na Android 6,0 ali novejšo.

3. Onesposobiti hrust spreten šef s upraven InTune družba portal. Preglejte [ta dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za več podrobnosti o teh vprašanjih in resolucijah.

 **Uporabniška licenčna vrsta neveljavna** ali **uporabniško ime ni prepoznana napaka:** uporabniku je treba dodeliti licenco InTune ali EMS. Preglejte te dokumente, če želite dodeliti licenco prek: Officeovega skrbniškega središča ali portala Azure.
  
Dodatni viri, ki vam pomagajo odpraviti težavo:
  
1. Uporabite [InTune odpravljanje težav portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za diagnosticiranje in reševanje pogostih napak včlanitve. Za več podrobnosti preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .

2. Preglejte [ta dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za seznam pogostih napak, ki preprečujejo včlanitev in resolucije vsakemu.

3. [Naučite se včlaniti naprave Android v Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).
