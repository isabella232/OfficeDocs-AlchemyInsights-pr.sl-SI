---
title: Odpravljanje težav z vpisom naprav Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661578"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Odpravljanje težav z vpisom naprav Windows Microsoft Intune

Pregledati vire spodaj za zdaj rešiti težavo. 
  
Neki splošen zmota vest ter odložnost lestev:
  
 **Programske opreme ni mogoče namestiti, 0x80cf4017:** Vaš račun potrdilo je poteklo. Drugi ton oktave-travnato gričevje PC odjemalca programski paket v Admin konzoli Intune. Pregled ta dokumentacija za več informacij. 
  
 **Zmota zbornik 0x801c0003:** Napaka se lahko pojavi v naslednjih primerih: 
  
1. Uporabnik ima več naprav, ki so vpisani presega omejitev naprave. Pregled teh dokumentov [odstranite napravo](https://docs.microsoft.com/intune/devices-wipe) ali [spremeniti omejitev naprave](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. »Uporabniki lahko pridružijo naprave Azure oglas« nastavljen na "brez". Jo nastavite na vse ali izberite Uporabniki. Pregled [ta dokumentacija](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za več informacij. 
    
3. Naprava je vpisan že drug uporabnik. Če je temu tako, odstranite napravo iz Azure Intune konzole ali ročno izpisati napravo, preden poskusite znova.
    
4. Naprava je Windows 10 domov. Samo okno 10 Pro, izobraževanje in podjetja SKUs lahko pridruži Azure storitve Active Directory.
    
Dodatna sredstva za pomoč pri reševanju težave:
  
1. Uporabite [Intune odpravljanje težav Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnosticirati in odpraviti skupni vpis napak. Pregled [tega dokumenta](https://docs.microsoft.com/intune/help-desk-operators) za več podrobnosti. 
    
2. Pregled teh dokumentov seznam pogostih napak, ki preprečujejo včlanitev in resolucije posameznim: [Priročnik za odpravljanje težav](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) in [Odpravljanje težav doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Naučite se, kako vpisati naprav Windows Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

