---
title: Odpravljanje težav pri včlanitvi naprav s sistemom iOS v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823479"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Odpravljanje težav pri včlanitvi naprav s sistemom iOS v Microsoft Intune

Preglejte vire spodaj, da odpravite težavo. 
  
Nekatera pogosta sporočila o napakah in koraki za odpravljanje težav:
  
- **Dosežena je bila kapa naprave** Uporabnik ima včlanitev več naprav, kot je omejitev naprave. Preglejte te [dokumente, da odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali spremenite omejitev [naprave.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ta storitev ni podprta. Brez pravilnika o včlanitve:** storitev potisnih obvestil Apple Push Notification Service (APNS) je treba konfigurirati ali obnoviti. Preglejte [ta dokument,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) če želite navodila, kako to naredite. 
    
- **Vrsta uporabniške licence Neveljavno ali Uporabniško ime ni prepoznano:** Uporabniku mora biti dodeljena licenca za Intune ali EMS. Preglejte te dokumente, da dodelite licenco prek: [Skrbniškega središča za Office](https://docs.microsoft.com/intune/licenses-assign) ali [portala Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Dodatni viri za odpravljanje težave:
  
1. S [portalom za odpravljanje težav za Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lahko diagnosticirate in odpravite pogoste napake z včlani. Preglejte [ta dokument,](https://docs.microsoft.com/intune/help-desk-operators) če želite več podrobnosti. 
    
2. V dokumentih si oglejte seznam pogostih napak, ki preprečujejo včlanitev in rešitve za posamezne uporabnike: Vodnik za odpravljanje težav [in](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) [Odpravljanje težav z dokumentom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Preberite, kako včlanite naprave s sistemom iOS v Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

