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
# <a name="teams-client-crashing"></a><span data-ttu-id="f9067-102">Ali se je odjemalec aplikacije Teams sesul?</span><span class="sxs-lookup"><span data-stu-id="f9067-102">Teams client crashing?</span></span>

<span data-ttu-id="f9067-103">Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="f9067-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="f9067-104">Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="f9067-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="f9067-105">Preverite, ali so vsi URL-ji in obsegi naslovov za [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) dostopni.</span><span class="sxs-lookup"><span data-stu-id="f9067-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="f9067-106">Prijavite se s skrbniškim računom [](https://docs.microsoft.com/office365/enterprise/view-service-health) najemnika in preverite nadzorno ploščo stanja storitve, da preverite, ali ne obstaja degradacija sistema ali delovanja storitve.</span><span class="sxs-lookup"><span data-stu-id="f9067-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="f9067-107">Odstranitev in ponovna namestitev aplikacije Teams (povezava)</span><span class="sxs-lookup"><span data-stu-id="f9067-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="f9067-108">Poiščite mapo %appdata%\Microsoft\teams\ v računalniku in izbrišite vse datoteke v tem imeniku.</span><span class="sxs-lookup"><span data-stu-id="f9067-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="f9067-109">Prenesite in [namestite aplikacijo Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)ter, če je mogoče, namestite aplikacijo Teams kot skrbnik (z desno tipko miške kliknite namestitveni program Teams in izberite »Zaženi kot skrbnik«, če je na voljo).</span><span class="sxs-lookup"><span data-stu-id="f9067-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="f9067-110">Ali lahko ponovno ustvarite težavo, če se odjemalec storitve Teams še vedno zruši?</span><span class="sxs-lookup"><span data-stu-id="f9067-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="f9067-111">V tem primeru:</span><span class="sxs-lookup"><span data-stu-id="f9067-111">If so:</span></span>

1. <span data-ttu-id="f9067-112">S Snemalnikom korakov posnemite svoje korake.</span><span class="sxs-lookup"><span data-stu-id="f9067-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="f9067-113">Zaprite vse nepotrebne ali zaupne programe.</span><span class="sxs-lookup"><span data-stu-id="f9067-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="f9067-114">Zaženite snemalnik korakov in ponovno prinjujte težavo, medtem ko ste prijavljeni s tem uporabniškim računom.</span><span class="sxs-lookup"><span data-stu-id="f9067-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="f9067-115">[Zberite dnevnike skupin, ki zajamejo posnete korake za ponovitev.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="f9067-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="f9067-116">**Opomba:** Zabeležite naslov za vpis uporabnika, na katerega to vpliva.</span><span class="sxs-lookup"><span data-stu-id="f9067-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="f9067-117">Zberite informacije o izvozu in/ali vedro napak (Windows).</span><span class="sxs-lookup"><span data-stu-id="f9067-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="f9067-118">Zaženite Windows Powershell v računalniku, v katerem se zruši, in zaženite te ukaze:</span><span class="sxs-lookup"><span data-stu-id="f9067-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="f9067-119">Priložite datoteko primeru podpore.</span><span class="sxs-lookup"><span data-stu-id="f9067-119">Attach the file to your support case.</span></span>
