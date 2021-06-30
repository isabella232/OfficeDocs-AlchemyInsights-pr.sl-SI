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
# <a name="teams-client-crashing"></a><span data-ttu-id="9ca73-102">Teams odjemalca se zruši</span><span class="sxs-lookup"><span data-stu-id="9ca73-102">Teams client crashing</span></span>

<span data-ttu-id="9ca73-103">Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="9ca73-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="9ca73-104">Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="9ca73-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="9ca73-105">Prepričajte se, da [Microsoft 365 vsi URL-ji](/microsoftteams/connectivity-issues) in obsegi naslovov dostopni.</span><span class="sxs-lookup"><span data-stu-id="9ca73-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="9ca73-106">Prijavite se s skrbniškim računom [](/office365/enterprise/view-service-health) najemnika in preverite nadzorno ploščo stanja storitve, da preverite, ali ne obstaja degradacija sistema ali delovanja storitve.</span><span class="sxs-lookup"><span data-stu-id="9ca73-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="9ca73-107">Odstranitev in ponovna namestitev Teams programa</span><span class="sxs-lookup"><span data-stu-id="9ca73-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="9ca73-108">Poiščite mapo %appdata%\Microsoft\Teams\ v računalniku in izbrišite vse datoteke v tem imeniku.</span><span class="sxs-lookup"><span data-stu-id="9ca73-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="9ca73-109">Prenesite in [namestite Teams aplikacijo](https://www.microsoft.com/microsoft-teams/download-app)in, če je mogoče, namestite Teams kot skrbnik (z desno  tipko miške kliknite namestitveni program storitve Teams in izberite Zaženi kot skrbnik, če je na voljo).</span><span class="sxs-lookup"><span data-stu-id="9ca73-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="9ca73-110">Če se Teams odjemalca še vedno sesuva, poskusite znova prišteti težavo.</span><span class="sxs-lookup"><span data-stu-id="9ca73-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="9ca73-111">Če lahko:</span><span class="sxs-lookup"><span data-stu-id="9ca73-111">If you can:</span></span>

1. <span data-ttu-id="9ca73-112">S Snemalnikom korakov posnemite svoje korake.</span><span class="sxs-lookup"><span data-stu-id="9ca73-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="9ca73-113">Zaprite vse nepotrebne ali zaupne programe.</span><span class="sxs-lookup"><span data-stu-id="9ca73-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="9ca73-114">Zaženite snemalnik korakov in ponovno prinjujte težavo, medtem ko ste prijavljeni s tem uporabniškim računom.</span><span class="sxs-lookup"><span data-stu-id="9ca73-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="9ca73-115">[Zberite dnevnike skupin, ki zajamejo posnete korake za ponovitev.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="9ca73-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="9ca73-116">**Opomba:** Zabeležite naslov za vpis uporabnika, na katerega to vpliva.</span><span class="sxs-lookup"><span data-stu-id="9ca73-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="9ca73-117">Zberite informacije o izvozu in/ali vedro napake (Windows).</span><span class="sxs-lookup"><span data-stu-id="9ca73-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="9ca73-118">Zaženite Windows Powershell v računalniku, v katerem se pojavlja zrušitev, in zaženite te ukaze (po vsakem ukazu pritisnite Enter):</span><span class="sxs-lookup"><span data-stu-id="9ca73-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="9ca73-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="9ca73-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="9ca73-120">Ko ustvarite besedilno datoteko in se prikaže na zaslonu, shranite datoteko in jo priložite zahtevam storitve.</span><span class="sxs-lookup"><span data-stu-id="9ca73-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
