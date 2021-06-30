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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187737"
---
# <a name="teams-client-crashing"></a>Teams odjemalca se zruši

Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:

- Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Prepričajte se, da [Microsoft 365 vsi URL-ji](/microsoftteams/connectivity-issues) in obsegi naslovov dostopni.

- Prijavite se s skrbniškim računom [](/office365/enterprise/view-service-health) najemnika in preverite nadzorno ploščo stanja storitve, da preverite, ali ne obstaja degradacija sistema ali delovanja storitve.

- Odstranitev in ponovna namestitev Teams programa
    - Poiščite mapo %appdata%\Microsoft\Teams\ v računalniku in izbrišite vse datoteke v tem imeniku.
    - Prenesite in [namestite Teams aplikacijo](https://www.microsoft.com/microsoft-teams/download-app)in, če je mogoče, namestite Teams kot skrbnik (z desno  tipko miške kliknite namestitveni program storitve Teams in izberite Zaženi kot skrbnik, če je na voljo).

Če se Teams odjemalca še vedno sesuva, poskusite znova prišteti težavo. Če lahko:

1. S Snemalnikom korakov posnemite svoje korake.
    - Zaprite vse nepotrebne ali zaupne programe.
    - Zaženite snemalnik korakov in ponovno prinjujte težavo, medtem ko ste prijavljeni s tem uporabniškim računom.
    - [Zberite dnevnike skupin, ki zajamejo posnete korake za ponovitev.](/microsoftteams/log-files) **Opomba:** Zabeležite naslov za vpis uporabnika, na katerega to vpliva.
    - Zberite informacije o izvozu in/ali vedro napake (Windows). Zaženite Windows Powershell v računalniku, v katerem se pojavlja zrušitev, in zaženite te ukaze (po vsakem ukazu pritisnite Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Ko ustvarite besedilno datoteko in se prikaže na zaslonu, shranite datoteko in jo priložite zahtevam storitve. 
