---
title: Odpravljanje težav z včlanjanjem naprav iOS v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507019"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Odpravljanje težav z včlanjanjem naprav iOS v Microsoft InTune

Preglejte spodaj navedene vire, da odpravite težavo zdaj. 
  
Nekatera pogosta sporočila o napakah in koraki reševanja:
  
- **Naprava SKP dosežena** Uporabnik ima več naprav, vpisanih kot omejitev naprave. Preglejte te dokumente, če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ta storitev ni podprta. Št vpis politika:** Apple push obvestilo Service (APNS) je treba konfigurirati ali obnoviti. Preglejte [ta dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , če želite navodila za to. 
    
- **Uporabniška licenčna vrsta neveljavna ali uporabniško ime ni bilo prepoznano:** Uporabniku je treba dodeliti licenco InTune ali EMS. Preglejte te dokumente, če želite dodeliti licenco prek: [Officeovega skrbniškega središča](https://docs.microsoft.com/intune/licenses-assign) ali [portala Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatni viri, ki vam pomagajo odpraviti težavo:
  
1. Uporabite [InTune odpravljanje težav portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za diagnosticiranje in reševanje pogostih napak včlanitve. Za več podrobnosti preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Preglejte te dokumente za seznam pogostih napak, ki preprečujejo včlanitev in resolucije vsakemu: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) in [Odpravljanje težav z zdravnikom](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Naučite se včlaniti naprave IOS v Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).
    

