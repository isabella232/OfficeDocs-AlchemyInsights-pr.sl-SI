---
title: Teams odjemalca se zruši
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890354"
---
# <a name="teams-client-crashing"></a>Teams odjemalca se zruši

Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:

- Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Preverite, ali so [vsi Microsoft 365 URL-ji in obsegi naslovov](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostopni.

- Prijavite se s skrbniškim računom [](https://docs.microsoft.com/office365/enterprise/view-service-health) najemnika in preverite nadzorno ploščo stanja storitve ter se prepričajte, da ne bo mogoče degradacije storitve ali delovanja storitve.

- Odstranitev in ponovna namestitev Teams programa
    - Poiščite mapo %appdata%\Microsoft\Teams\ v računalniku in izbrišite vse datoteke v tem imeniku.
    - Prenesite in [namestite aplikacijo Teams](https://www.microsoft.com/microsoft-teams/download-app)in, če je mogoče, namestite Teams kot skrbnik (z desno tipko miške kliknite namestitveni program storitve Teams in izberite Zaženi kot skrbnik, če je na voljo). 

Če se Teams odjemalca še vedno sesuva, poskusite znova prišteti težavo. Če lahko:

1. S Snemalnikom korakov posnemite svoje korake.
    - Zaprite vse nepotrebne ali zaupne programe.
    - Zaženite snemalnik korakov in ponovno prinjujte težavo, medtem ko ste prijavljeni s tem uporabniškim računom.
    - [Zberite dnevnike skupin, ki zajamejo posnete korake za ponovitev.](https://docs.microsoft.com/microsoftteams/log-files) **Opomba:** Zabeležite naslov za vpis uporabnika, na katerega to vpliva.
    - Zberite informacije o izvozu in/ali vedro napake (Windows). Zaženite Windows Powershell v računalniku, v katerem se pojavlja zrušitev, in zaženite te ukaze (po vsakem ukazu pritisnite Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Ko ustvarite besedilno datoteko in se prikaže na zaslonu, shranite datoteko in jo priložite zahtevam storitve. 
