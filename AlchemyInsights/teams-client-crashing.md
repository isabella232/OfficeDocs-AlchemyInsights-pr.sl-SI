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
# <a name="teams-client-crashing"></a><span data-ttu-id="eb482-102">Ali se je odjemalec aplikacije Teams sesul?</span><span class="sxs-lookup"><span data-stu-id="eb482-102">Teams client crashing?</span></span>

<span data-ttu-id="eb482-103">Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="eb482-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="eb482-104">Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="eb482-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="eb482-105">Poskrbite, da bodo vsi [spletni naslovi in naslovi naslovov Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostopni.</span><span class="sxs-lookup"><span data-stu-id="eb482-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="eb482-106">Prijavite se z računom skrbnika za najemnike in preverite, ali je na voljo [Nadzorna plošča storitve](https://docs.microsoft.com/office365/enterprise/view-service-health) , da preverite, ali degradacija ali storitev ne obstaja.</span><span class="sxs-lookup"><span data-stu-id="eb482-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="eb482-107">Odstranite in znova namestite aplikacijo Teams (povezava)</span><span class="sxs-lookup"><span data-stu-id="eb482-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="eb482-108">Prebrskajte do mape%appdata%\Microsoft\teams\ v računalniku in izbrišite vse datoteke v tem imeniku.</span><span class="sxs-lookup"><span data-stu-id="eb482-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="eb482-109">[Prenesite in namestite aplikacijo Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)in po možnosti namestite ekipe kot skrbnika (z desno miškino tipko kliknite namestitveni program in izberite» Zaženi kot skrbnik «, če je na voljo).</span><span class="sxs-lookup"><span data-stu-id="eb482-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="eb482-110">Če je vaš stranka ekipe še vedno treskav, lahko to vprašanje reproducira?</span><span class="sxs-lookup"><span data-stu-id="eb482-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="eb482-111">Če je tako:</span><span class="sxs-lookup"><span data-stu-id="eb482-111">If so:</span></span>

1. <span data-ttu-id="eb482-112">Če želite zajeti korake, uporabite snemalnik korakov.</span><span class="sxs-lookup"><span data-stu-id="eb482-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="eb482-113">Zaprite vse nepotrebne ali zaupne aplikacije.</span><span class="sxs-lookup"><span data-stu-id="eb482-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="eb482-114">Zaženite snemalnik korakov in reproducirati težavo, medtem ko prijavljeni z prizadetim uporabniškim računom.</span><span class="sxs-lookup"><span data-stu-id="eb482-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="eb482-115">[Zbirajo ekipe dnevniki, ki zajemajo posnete REPRO korake](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="eb482-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="eb482-116">**Opomba**: poskrbite, da boste zajeli vpisni naslov vplivnega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="eb482-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="eb482-117">Zbirajte smetišče in/ali informacije o vedro napake (Windows).</span><span class="sxs-lookup"><span data-stu-id="eb482-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="eb482-118">Zaženite Windows PowerShell na stroju, kjer se pojavlja nesreča in zaženite naslednje ukaze:</span><span class="sxs-lookup"><span data-stu-id="eb482-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="eb482-119">Priložite datoteko v primer podpore.</span><span class="sxs-lookup"><span data-stu-id="eb482-119">Attach the file to your support case.</span></span>
