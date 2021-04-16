---
title: Odpravljanje težav z včlanijo naprav s sistemom Windows v storitvi Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808987"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Odpravljanje težav z včlanijo naprav s sistemom Windows v storitvi Microsoft Intune

Preglejte vire spodaj, da odpravite težavo.
  
Nekatera pogosta sporočila o napakah in koraki za odpravljanje težav:
  
 **Programske opreme ni mogoče namestiti, 0x80cf4017:** Potrdilo računa je poteklo. Znova prenesite paket programske opreme odjemalca za PC v skrbniški konzoli za Intune. Če želite več informacij, si oglejte to dokumentacijo.
  
 **Koda napake 0x801c0003:** Do napake lahko pride v teh primerih:
  
-  Uporabnik ima včlanitev več naprav, kot je omejitev naprave. Preglejte te [dokumente, da odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali spremenite omejitev [naprave.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  »Uporabniki lahko naprave pridružijo imeniku Azure AD« je nastavljen na »brez«. Nastavite jo za vse ali izberite uporabnike. Če [želite več informacij,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) si oglejte to dokumentacijo.

-  Napravo že včlani drug uporabnik. V tem primeru odstranite napravo iz konzole Azure Intune ali ročno odstranite napravo, preden poskusite znova.

-  Naprava je Windows 10 Home. Imeniku Azure Active Directory se lahko pridružijo le inventavne datoteke (SK) za Windows 10 Pro, Education in Enterprise.

Dodatni viri za odpravljanje težave:
  
-  S [portalom za odpravljanje težav za Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lahko diagnosticirate in odpravite pogoste napake z včlani. Preglejte [ta dokument,](https://docs.microsoft.com/intune/help-desk-operators) če želite več podrobnosti.

-  V dokumentih si oglejte seznam pogostih napak, ki preprečujejo včlanitev in rešitve za posamezne uporabnike: Vodnik za odpravljanje težav [in](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) [Odpravljanje težav z dokumentom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Preberite, kako včlanite naprave s sistemom Windows v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
