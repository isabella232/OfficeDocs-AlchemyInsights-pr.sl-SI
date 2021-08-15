---
title: Odpravljanje težav z včlani Windows v Microsoft Intune
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
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981057"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Odpravljanje težav z včlani Windows v Microsoft Intune

Preglejte vire spodaj, da odpravite težavo.
  
Nekatera pogosta sporočila o napakah in koraki za odpravljanje težav:
  
 **Programske opreme ni mogoče namestiti, 0x80cf4017:** Potrdilo računa je poteklo. Znova prenesite paket programske opreme odjemalca za PC v skrbniški konzoli za Intune. Če želite več informacij, si oglejte to dokumentacijo.
  
 **Koda napake 0x801c0003:** Do napake lahko pride v teh primerih:
  
-  Uporabnik ima včlanitev več naprav, kot je omejitev naprave. Preglejte te [dokumente, da odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali spremenite omejitev [naprave.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  »Uporabniki lahko naprave pridružijo imeniku Azure AD« je nastavljen na »brez«. Nastavite jo za vse ali izberite uporabnike. Če [želite več informacij,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) si oglejte to dokumentacijo.

-  Napravo že včlani drug uporabnik. V tem primeru odstranite napravo iz konzole Azure Intune ali ročno odstranite napravo, preden poskusite znova.

-  Naprava je Windows 10 Home. Le Windows 10 Pro se lahko pridružijo inventarno poročilo za izobraževanje in velika poslovna Azure Active Directory.

Dodatni viri za odpravljanje težave:
  
-  S [portalom za odpravljanje težav za Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lahko diagnosticirate in odpravite pogoste napake z včlani. Preglejte [ta dokument,](https://docs.microsoft.com/intune/help-desk-operators) če želite več podrobnosti.

-  Preglejte te dokumente in si oglejte seznam pogostih napak, ki preprečujejo včlanitev, in rešitev za posamezne težave: [Vodnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Dokument za odpravljanje težav](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Preberite, kako včlanite Windows v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
