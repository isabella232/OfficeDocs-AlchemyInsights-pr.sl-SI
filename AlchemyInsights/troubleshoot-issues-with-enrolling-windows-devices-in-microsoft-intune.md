---
title: Odpravljanje težav z včlanjanjem v naprave s sistemom Windows v programu Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665848"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Odpravljanje težav z včlanjanjem v naprave s sistemom Windows v programu Microsoft InTune

Preglejte spodaj navedene vire, da odpravite težavo zdaj.
  
Nekatera pogosta sporočila o napakah in koraki reševanja:
  
 **Programske opreme ni mogoče namestiti, 0x80cf4017:** Potrdilo o računu je poteklo. Re-Download PC Client paket programske opreme v InTune admin Console. Za več informacij preglejte to dokumentacijo.
  
 **Koda napake 0x801c0003:** Napaka se lahko pojavi v naslednjih scenarijih:
  
-  Uporabnik ima več naprav, vpisanih kot omejitev naprave. Preglejte te dokumente, če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Uporabnik maj združiti načrt v Azure AD" je število enakih oseb v "nič". Nastavite jo na vse ali izberite uporabnike. Če želite več informacij, preglejte [to dokumentacijo](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Napravo je že vpisal drug uporabnik. V tem primeru odstranite napravo iz konzole Azure InTune ali ročno izvlecite napravo, preden znova poskušate.

-  Naprava je Windows 10 Home. V Azure Active Directory se lahko pridružijo samo Windows 10 Pro, izobraževanje in Enterprise SKUs.

Dodatni viri, ki vam pomagajo odpraviti težavo:
  
-  Uporabite [InTune odpravljanje težav portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) za diagnosticiranje in reševanje pogostih napak včlanitve. Za več podrobnosti preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .

-  Preglejte te dokumente za seznam pogostih napak, ki preprečujejo včlanitev in resolucije vsakemu: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Odpravljanje težav z zdravnikom](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Naučite se včlaniti naprave Windows v Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).
