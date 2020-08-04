---
title: Uporaba e-poštnih profilov s storitvijo Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555761"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="47bbb-102">Uporaba e-poštnih profilov s storitvijo Intune</span><span class="sxs-lookup"><span data-stu-id="47bbb-102">Using email profiles with Intune</span></span>

<span data-ttu-id="47bbb-103">Intune se lahko uporablja za ustvarjanje in uvajanje e-poštnih profilov za izvornega (vgrajenega) e-poštnega odjemalca na več platformah naprav.</span><span class="sxs-lookup"><span data-stu-id="47bbb-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="47bbb-104">Če želite več informacij o nekaterih omejitvah, povezanih z e-poštnimi profili, vključno s tem, kako se obravnava prisotnost obstoječih profilov in kako [odstraniti e-poštne profile, glejte Dodajanje e-poštnih nastavitev napravam s storitvijo Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="47bbb-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="47bbb-105">Če želite več informacij o ustvarjanju e-poštnih profilov za vsako platformo naprave, glejte:</span><span class="sxs-lookup"><span data-stu-id="47bbb-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="47bbb-106">Nastavitve naprave Android za konfiguracijo e-pošte, preverjanja pristnosti in sinhronizacije v intunu</span><span class="sxs-lookup"><span data-stu-id="47bbb-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="47bbb-107">Dodajanje nastavitev e-pošte za naprave s sistemom iOS in iPadOS v storitvi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="47bbb-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="47bbb-108">Nastavitve e-poštnega profila v storitvi Microsoft Intune za naprave s sistemom Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="47bbb-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="47bbb-109">Nastavitve e-poštnega profila za naprave s sistemom Windows 10 v storitvi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="47bbb-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="47bbb-110">**Pogosta težava pri sinhronizaciji**</span><span class="sxs-lookup"><span data-stu-id="47bbb-110">**Common syncing issue**</span></span>

<span data-ttu-id="47bbb-111">**Knox v e-poštnem profilu za Android preprečuje sinhronizacijo uporabniških stikov, koledarja in opravil z uporabniškimi napravami.**</span><span class="sxs-lookup"><span data-stu-id="47bbb-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="47bbb-112">Knox na Android Knox e-poštni profil ponuja admin možnost, da se odločijo, katere vrste vsebine so sync'd z napravo z nastavitvijo vsak omogočen.</span><span class="sxs-lookup"><span data-stu-id="47bbb-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="47bbb-113">Če je nastavitev za katero koli od vrst vsebine **nastavljena na Ni konfigurirano** (privzeto), se ta vrsta vsebine ne sinhronizira samodejno.</span><span class="sxs-lookup"><span data-stu-id="47bbb-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="47bbb-114">Uporabnik lahko omogoči vrsto vsebine, ki jo želijo, neposredno v napravi ročno, vendar je ta konfiguracija prepisana z nastavitvijo pravilnika Intune, sinhronizacija pa se ustavi za to vrsto vsebine.</span><span class="sxs-lookup"><span data-stu-id="47bbb-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

