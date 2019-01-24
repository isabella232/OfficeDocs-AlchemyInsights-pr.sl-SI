---
title: Odpravljanje težav z vpisom Android naprave v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29489884"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Odpravljanje težav z vpisom Android naprave v Microsoft Intune

Pregledati vire spodaj za zdaj rešiti težavo.
  
Nekatere pogoste težave in odložnost lestev:
  
 **Naprave niso šifrirani napake v podjetje Portal:** Nove različice Android, zlasti začenši s v7.0, zahtevajo zagonsko kodo, se prepričajte, da naprava je popolnoma šifrirano. So skupne rešitve omogočajo zagonski pin ali popolnoma šifriranje naprave. Pregled [tega dokumenta](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za več informacij. 
  
 **Naprave ne preverite s storitvijo Intune ali prikazati kot "Nezdrava" v admin konzoli Intune:** Nekatere Samsung 4,4 in 5,5 naprave lahko preverja v storitev. Obstajajo 3 možne rešitve za to težavo: 
  
1. Ročno odprite app Intune podjetje Portal, ki bo samodejno sproži načrt omedlevičen.
    
2. Posodobitev naprave Android 6,0 ali višje.
    
3. Onesposobiti Samsung pameten šef od upravljanja Intune podjetje Portal. Pregled [tega dokumenta](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za več podrobnosti o teh vprašanjih in resolucij. 
    
 **Uporabnik dati dovoljenje vrsta neveljavne** ali **uporabniško ime ni prepoznano napaka:** uporabnik potrebuje dodelijo licenco Intune ali EMS. Pregled teh dokumentov dodeliti licenco skozi: Office Admin Center ali Azure portal. 
  
Dodatna sredstva za pomoč pri reševanju težave:
  
1. Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak. Pregled [tega dokumenta](https://docs.microsoft.com/en-us/intune/help-desk-operators) za več podrobnosti. 
    
2. Pregled [tega dokumenta](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za seznam pogostih napak, ki preprečujejo včlanitev in resolucije za vsako. 
    
3. [Naučite se, kako vpisati Android naprave v Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).
    

