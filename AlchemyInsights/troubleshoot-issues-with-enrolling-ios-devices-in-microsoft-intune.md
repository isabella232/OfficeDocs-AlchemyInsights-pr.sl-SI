---
title: Odpravljanje težav z vpisom naprav s sistemom iOS v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708978"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Odpravljanje težav z vpisom naprav s sistemom iOS v Microsoft InTune

Preglejte spodaj navedene vire, da odpravite težavo zdaj. 
  
Nekaj pogostih sporočil o napaki in korakih reševanja:
  
- **Dosežen je bil pokrovček naprave** Uporabnik ima več naprav, ki so bile včlanjene kot omejitev naprave. Če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), preglejte te dokumente.
    
- **Ta storitev ni podprta. Št pravilnik o vpisu:** storitev Apple push Service (APNS) mora biti konfigurirana ali obnovljena. Oglejte si [ta dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , če želite navodila o tem, kako to naredite. 
    
- **Vrsta uporabniške licence ni veljavna ali pa uporabniško ime ni prepoznano:** Uporabniku je treba dodeliti licenco za InTune ali EMS. Preglejte te dokumente, če želite dodeliti licenco prek [skrbniškega središča za Office](https://docs.microsoft.com/intune/licenses-assign) ali [portala Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatni viri za pomoč pri reševanju težave:
  
1. V [portalu za odpravljanje težav](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) s težavo lahko diagnosticirate in odpravite pogoste napake pri vpisu. Če želite več podrobnosti, preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Preglejte te dokumente za seznam pogostih napak, ki preprečujejo vpis in resolucije za vsako: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) in [Odpravljanje težav z doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Naučite se vpisati naprave s sistemom IOS v Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).
    

