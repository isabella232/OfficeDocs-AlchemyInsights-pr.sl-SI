---
title: Pomoč pri nastavitvi prikaza nočne svetlobe
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
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405181"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="0e0e0-102">Pomoč pri nastavitvi prikaza nočne svetlobe</span><span class="sxs-lookup"><span data-stu-id="0e0e0-102">Help with the night light display setting</span></span>

<span data-ttu-id="0e0e0-103">Če želite izvedeti več o nastavitvah zaslona za nočni čas, [glejte Nastavitev zaslona za nočni čas v sistemu Windows 10.](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)</span><span class="sxs-lookup"><span data-stu-id="0e0e0-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="0e0e0-104">Če so možnosti nočne svetlobe zatemnjene v nastavitvah, preverite gonilnik zaslona:</span><span class="sxs-lookup"><span data-stu-id="0e0e0-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="0e0e0-105">Kliknite iskalno polje v opravilni vrstici in **vnesite Upravitelj** naprav ter med **rezultati iskanja** izberite Upravitelj naprav.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="0e0e0-106">Razširi **grafične kartice.**</span><span class="sxs-lookup"><span data-stu-id="0e0e0-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="0e0e0-107">Žal funkcija nočne svetlobe ni na voljo, če vaša naprava uporablja gonilnik DisplayLink ali osnovni gonilnik grafične kartice.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="0e0e0-108">Funkcija nočne svetlobe uporablja nedavno grafično tehnologijo, zato boste morda morali posodobiti gonilnik grafične kartice:</span><span class="sxs-lookup"><span data-stu-id="0e0e0-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="0e0e0-109">Če želite preveriti, ali so na **voljo** posodobitve, izberite Začni  >    >  **posodobitev nastavitev & Windows**  >  **Update Preveri,** ali so na voljo  >  **posodobitve.**</span><span class="sxs-lookup"><span data-stu-id="0e0e0-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="0e0e0-110">OR</span><span class="sxs-lookup"><span data-stu-id="0e0e0-110">OR</span></span>

- <span data-ttu-id="0e0e0-111">Obiščite spletno mesto podpore izdelovalca strojne opreme, da ročno prenesete in namestite najnovejše gonilnike grafične opreme.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="0e0e0-112">Ponastavitev nočne svetlobe v registru</span><span class="sxs-lookup"><span data-stu-id="0e0e0-112">Reset night light in the registry</span></span>

<span data-ttu-id="0e0e0-113">Če posodobitev gonilnika grafične kartice ni delovala, boste morda morali ponastaviti nočno svetlobo v registru.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="0e0e0-114">**Pozor:** Ta korak za odpravljanje težav priporočamo le izkušenim uporabnikom.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="0e0e0-115">Če register spremenite nepravilno, lahko pride do resnih težav.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="0e0e0-116">Za dodatno varnost pred spreminjanjem registra varnostno kopijo registra, da ga lahko obnovite, če pride do težav.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="0e0e0-117">V iskalno polje vnesite **regedit** in med rezultati **iskanja izberite Urejevalnik** registra.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="0e0e0-118">Pojdite na ta registrski ključ:</span><span class="sxs-lookup"><span data-stu-id="0e0e0-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="0e0e0-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="0e0e0-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="0e0e0-120">Izvozite in izbrišite ta podključ:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="0e0e0-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="0e0e0-121">Izvozite in izbrišite ta podključ:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="0e0e0-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="0e0e0-122">Znova zaženite Windows in preverite, ali so na voljo možnosti nočne svetlobe.</span><span class="sxs-lookup"><span data-stu-id="0e0e0-122">Restart Windows and verify if the night light options are available.</span></span>


