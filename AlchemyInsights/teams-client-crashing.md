---
title: Ali se je odjemalec aplikacije Teams sesul?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354069"
---
# <a name="teams-client-crashing"></a>Ali se je odjemalec aplikacije Teams sesul?

Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:

- Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Poskrbite, da bodo vsi [spletni naslovi in naslovi naslovov Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostopni.

- Prijavite se z računom skrbnika za najemnike in preverite, ali je na voljo [Nadzorna plošča storitve](https://docs.microsoft.com/office365/enterprise/view-service-health) , da preverite, ali degradacija ali storitev ne obstaja.

- Odstranite in znova namestite aplikacijo Teams (povezava)
    - Prebrskajte do mape%appdata%\Microsoft\teams\ v računalniku in izbrišite vse datoteke v tem imeniku.
    - [Prenesite in namestite aplikacijo Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)in po možnosti namestite ekipe kot skrbnika (z desno miškino tipko kliknite namestitveni program in izberite» Zaženi kot skrbnik «, če je na voljo).

Če je vaš stranka ekipe še vedno treskav, lahko to vprašanje reproducira? Če je tako:

1. Če želite zajeti korake, uporabite snemalnik korakov.
    - Zaprite vse nepotrebne ali zaupne aplikacije.
    - Zaženite snemalnik korakov in reproducirati težavo, medtem ko prijavljeni z prizadetim uporabniškim računom.
    - [Zbirajo ekipe dnevniki, ki zajemajo posnete REPRO korake](https://docs.microsoft.com/microsoftteams/log-files). **Opomba**: poskrbite, da boste zajeli vpisni naslov vplivnega uporabnika.
    - Zbirajte smetišče in/ali informacije o vedro napake (Windows). Zaženite Windows PowerShell na stroju, kjer se pojavlja nesreča in zaženite naslednje ukaze:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložite datoteko v primer podpore.
