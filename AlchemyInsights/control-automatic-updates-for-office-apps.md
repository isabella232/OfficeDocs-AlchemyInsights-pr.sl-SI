---
title: Nadzor samodejnih posodobitev za Officeove programe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439925"
---
# <a name="control-automatic-updates-for-office-apps"></a>Nadzor samodejnih posodobitev za Officeove programe

Posodobitve za Officeove aplikacije se privzeto samodejno prenesejo in uporabijo v ozadju brez posredovanja uporabnika. Vendar pa lahko skrbniki nadzirajo, kako se posodobitve uporabljajo z nastavitvami storitve Office Update. Nastavitve posodobitve skrbnikom omogočajo, da omogočijo ali onemogočijo samodejne posodobitve, **prikažejo ali skrijejo gumb Posodobi zdaj** v Officeu, nastavijo roke za posodobitev in še več. Za podrobnejše informacije glej:

- [Konfiguracija nastavitev posodobitve za Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Samodejno posodabljanje za Office ni omogočeno](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Določanje načina posodablja glede na to, kako se Office posodobi po namestitvi](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Če želite pregledati obstoječe nastavitve posodobitev, ki veljajo za odjemalski računalnik, sledite tem korakom:

1. plan registracija urednik z tekoč v **začetek prost**  >  **dostop**  >  **zopet zmrzniti**.
2. Preklopite na to mesto in preglejte nastavitve storitve Office Update:  
    A. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    B. Kliknite »Run\Configuration«

** Opomba**  Če je ključ OfficeMgmtCOM nastavljen, se lahko v officeovih posodobitvah za račun officea prikaže sporočilo **»Posodobitve**upravlja skrbnik  >  **Account**  >  **sistema«.** Če želite več informacij, [glejte Upravljanje posodobitev za programe Microsoft 365 z Microsoft Endpoint Configuration Managerjem](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  