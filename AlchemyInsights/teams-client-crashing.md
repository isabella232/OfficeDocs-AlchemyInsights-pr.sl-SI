---
title: Ali se je odjemalec aplikacije Teams sesul?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826287"
---
# <a name="teams-client-crashing"></a>Ali se je odjemalec aplikacije Teams sesul?

Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:

- Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Preverite, ali so vsi URL-ji in obsegi naslovov za [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostopni.

- Prijavite se s skrbniškim računom [](https://docs.microsoft.com/office365/enterprise/view-service-health) najemnika in preverite nadzorno ploščo stanja storitve, da preverite, ali ne obstaja degradacija sistema ali delovanja storitve.

- Odstranitev in ponovna namestitev aplikacije Teams (povezava)
    - Poiščite mapo %appdata%\Microsoft\teams\ v računalniku in izbrišite vse datoteke v tem imeniku.
    - Prenesite in [namestite aplikacijo Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ter, če je mogoče, namestite aplikacijo Teams kot skrbnik (z desno tipko miške kliknite namestitveni program Teams in izberite »Zaženi kot skrbnik«, če je na voljo).

Ali lahko ponovno ustvarite težavo, če se odjemalec storitve Teams še vedno zruši? V tem primeru:

1. S Snemalnikom korakov posnemite svoje korake.
    - Zaprite vse nepotrebne ali zaupne programe.
    - Zaženite snemalnik korakov in ponovno prinjujte težavo, medtem ko ste prijavljeni s tem uporabniškim računom.
    - [Zberite dnevnike skupin, ki zajamejo posnete korake za ponovitev.](https://docs.microsoft.com/microsoftteams/log-files) **Opomba:** Zabeležite naslov za vpis uporabnika, na katerega to vpliva.
    - Zberite informacije o izvozu in/ali vedro napak (Windows). Zaženite Windows Powershell v računalniku, v katerem se zruši, in zaženite te ukaze:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložite datoteko primeru podpore.
