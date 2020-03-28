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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030672"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="94b87-102">Ali se je odjemalec aplikacije Teams sesul?</span><span class="sxs-lookup"><span data-stu-id="94b87-102">Teams client crashing?</span></span>

<span data-ttu-id="94b87-103">Če se vaš odjemalec aplikacije Teams sesuje, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="94b87-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="94b87-104">Če uporabljate namizno aplikacijo Teams, [poskrbite, da bo aplikacija v celoti posodobljena](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="94b87-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="94b87-105">Prepričajte se, da so na voljo vsi [URL-ji in obsegi naslovov Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues).</span><span class="sxs-lookup"><span data-stu-id="94b87-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="94b87-106">Vpišite se s svojim skrbniškim računom in preverite [Nadzorne plošče za stanje storitve](https://docs.microsoft.com/office365/enterprise/view-service-health), da preverite, ali je prišlo do propada ali razgradnje storitve.</span><span class="sxs-lookup"><span data-stu-id="94b87-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="94b87-107">Kot zadnji korak lahko poskusite počistiti predpomnilnik odjemalca Teams:</span><span class="sxs-lookup"><span data-stu-id="94b87-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="94b87-108">Popolnoma zaprite namiznega odjemalca za Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="94b87-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="94b87-109">Z desno tipko miške kliknite **Teams** iz pladnja ikon in kliknite **zaprite**ali zaženite upravitelja opravil in popolnoma uničite postopek.</span><span class="sxs-lookup"><span data-stu-id="94b87-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="94b87-110">Pomaknite se v razdelek »raziskovalec datotek« in vnesite%appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="94b87-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="94b87-111">Ko ste v imeniku, boste videli nekaj teh map:</span><span class="sxs-lookup"><span data-stu-id="94b87-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="94b87-112">V **Predpomnilniku aplikacije**odprite predpomnilnik in izbrišite vse datoteke na mestu predpomnilnika:%appdata%\Microsoft\ teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="94b87-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="94b87-113">V **Blob_storage**izbrišite vse datoteke:%appdata%\Microsoft\teams\ blob_storage.</span><span class="sxs-lookup"><span data-stu-id="94b87-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="94b87-114">V **Predpomnilniku**, izbrišite vse datoteke:%appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="94b87-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="94b87-115">V **Zbirkah podatkov**izbrišite vse datoteke:%appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="94b87-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="94b87-116">V **GPUCache**izbrišite vse datoteke:%appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="94b87-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="94b87-117">V **IndexedDB**izbrišite datoteko. db:%appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="94b87-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="94b87-118">V **Lokalno shrambo**izbrišite vse datoteke: shramba%appdata%\Microsoft\teams\Local.</span><span class="sxs-lookup"><span data-stu-id="94b87-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="94b87-119">Nazadnje, v **tmp**, izbrišite poljubno datoteko:%appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="94b87-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="94b87-120">Znova zaženite odjemalca za aplikacijo Teams.</span><span class="sxs-lookup"><span data-stu-id="94b87-120">Restart your Teams client.</span></span>
