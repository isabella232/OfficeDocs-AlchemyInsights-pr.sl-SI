---
title: Odpravljanje težav z vpisom naprav sistema Windows v Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708906"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Odpravljanje težav z vpisom naprav sistema Windows v Microsoft InTune

Preglejte spodaj navedene vire, da odpravite težavo zdaj.
  
Nekaj pogostih sporočil o napaki in korakih reševanja:
  
 **Programske opreme ni mogoče namestiti, 0x80cf4017:** Potrdilo vašega računa je poteklo. Znova Prenesite programski paket odjemalca za računalnik s sistemom Windows v konzoli za InTune. Če želite več informacij, si oglejte to dokumentacijo.
  
 **Koda napake 0x801c0003:** Do napake lahko pride v teh primerih:
  
-  Uporabnik ima več naprav, ki so bile včlanjene kot omejitev naprave. Če želite [odstraniti napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions), preglejte te dokumente.

-  » Uporabniki lahko priključijo naprave na Azure AD «je nastavljena na» brez «. Nastavite vse ali izberite uporabnike. Če želite več informacij, si oglejte [to dokumentacijo](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Napravo je že vpisal drug uporabnik. Če je to res, odstranite napravo iz konzole Azure InTune ali pa jo ročno odpeljite, preden poskusite znova.

-  Naprava je Windows 10 Home. V storitvi Azure Active Directory se lahko pridružite le Windows 10 Pro, izobraževanje in podjetje SKUs.

Dodatni viri za pomoč pri reševanju težave:
  
-  V [portalu za odpravljanje težav](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) s težavo lahko diagnosticirate in odpravite pogoste napake pri vpisu. Če želite več podrobnosti, preglejte [ta dokument](https://docs.microsoft.com/intune/help-desk-operators) .

-  Preglejte te dokumente za seznam pogostih napak, ki preprečujejo vpis in resolucije za vsako: [vodnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Odpravljanje težav z doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Naučite se vpisati naprave s sistemom Windows v Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).
