---
title: Odpravljanje težav z vpisom iOS naprave v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: cd1afc83fe98f363aee4c3324a634c200cd08947
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658455"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Odpravljanje težav z vpisom iOS naprave v Microsoft Intune

Pregledati vire spodaj za zdaj rešiti težavo. 
  
Neki splošen zmota vest ter odložnost lestev:
  
- **Naprava SKP dosegel** Uporabnik ima več naprav, ki so vpisani presega omejitev naprave. Pregled teh dokumentov [odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ta storitev ni podprta. Noben vpis pravilnik:** Apple Push obvestila storitev (APNS) mora biti nastavljen ali podaljšati. Pregled [tega dokumenta](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za navodila o tem, kako to storiti. 
    
- **Uporabnik dati dovoljenje vrsta neveljavne ali uporabniško ime ni prepoznano:** Uporabnik potrebuje, dodelijo licenco Intune ali EMS. Pregled teh dokumentov dodeliti licenco skozi: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) ali [sinje portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatna sredstva za pomoč pri reševanju težave:
  
1. Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak. Pregled [tega dokumenta](https://docs.microsoft.com/intune/help-desk-operators) za več podrobnosti. 
    
2. Pregled teh dokumentov seznam pogostih napak, ki preprečujejo včlanitev in resolucije posameznim: [Priročnik za odpravljanje težav](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) in [Odpravljanje težav doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Naučite se, kako vpisati iOS naprave v Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

