---
title: Uporaba e-poštnih profilov s funkcijo InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653304"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="8940c-102">Uporaba e-poštnih profilov s funkcijo InTune</span><span class="sxs-lookup"><span data-stu-id="8940c-102">Using email profiles with Intune</span></span>

<span data-ttu-id="8940c-103">InTune lahko uporabite za ustvarjanje in uvajanje e-poštnih profilov za native (vgrajen) e-poštni odjemalec na več platformah naprav.</span><span class="sxs-lookup"><span data-stu-id="8940c-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="8940c-104">Če želite več informacij o nekaterih omejitvah, povezanih z e-poštnimi profili, vključno s tem, kako ravnati s prisotnostjo obstoječih profilov in kako odstraniti e-poštne profile, glejte [Dodajanje nastavitev e-pošte v naprave s funkcijo InTune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="8940c-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="8940c-105">Če želite več informacij o tem, kako ustvarite profile e-pošte za vsako platformo naprave, glejte:</span><span class="sxs-lookup"><span data-stu-id="8940c-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="8940c-106">Nastavitve naprave s sistemom Android za konfiguriranje e-pošte, preverjanja pristnosti in sinhronizacije v programu InTune</span><span class="sxs-lookup"><span data-stu-id="8940c-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="8940c-107">Dodajanje nastavitev e-pošte za naprave s sistemom iOS in iPadOS v programu Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="8940c-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="8940c-108">Nastavitve e-poštnega profila v Microsoft InTune za naprave s sistemom Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="8940c-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="8940c-109">Nastavitve e-poštnega profila za naprave s sistemom Windows 10 v programu Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="8940c-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="8940c-110">**Pogosta težava pri sinhronizaciji**</span><span class="sxs-lookup"><span data-stu-id="8940c-110">**Common syncing issue**</span></span>

<span data-ttu-id="8940c-111">**KNOX v e-poštnem profilu s sistemom Android preprečuje, da bi bile uporabniške stike, koledar in opravila sinhronizirane z uporabniškimi napravami.**</span><span class="sxs-lookup"><span data-stu-id="8940c-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="8940c-112">V oknu KNOX v telefonu s sistemom Android KNOX se lahko odločite, katere vrste vsebine bodo sinhronizirane z napravo, in sicer tako, da nastavite vsako možnost.</span><span class="sxs-lookup"><span data-stu-id="8940c-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="8940c-113">Če je nastavitev za katero koli vrsto vsebine nastavljena na **ni konfigurirana** (privzeta), ta vrsta vsebine ni samodejno sinhronizirana.</span><span class="sxs-lookup"><span data-stu-id="8940c-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="8940c-114">Uporabnik lahko želeno vrsto vsebine omogoči neposredno v napravi ročno, vendar je ta konfiguracija prepisana s nastavitev pravilnika InTune, sinhronizacije pa se ustavi za to vrsto vsebine.</span><span class="sxs-lookup"><span data-stu-id="8940c-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

