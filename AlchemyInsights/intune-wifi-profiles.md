---
title: Profili Intune Wi-Fi
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555814"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="effb2-102">Profili Intune Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="effb2-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="effb2-103">Uspešna izvedba povezljivosti Wi-Fi za odjemalce MDM je odvisna od pravilno uvedenega profila, ki odraža zahteve infrastrukture wi-fi podjetja.</span><span class="sxs-lookup"><span data-stu-id="effb2-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="effb2-104">Če želite pregledati ustrezne nastavitve za odjemalske platforme, ki jih preiskujete, glejte:</span><span class="sxs-lookup"><span data-stu-id="effb2-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="effb2-105">Dodajanje nastavitev omrežja Wi-Fi za naprave s sistemom Android v storitvi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="effb2-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="effb2-106">Dodajanje nastavitev wi-fi za namenske in v celoti upravljane naprave za Android Enterprise v storitvi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="effb2-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="effb2-107">Dodajanje nastavitev wi-fi za naprave s sistemom iOS in iPadOS v storitvi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="effb2-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="effb2-108">Dodajanje nastavitev omrežja Wi-Fi za naprave s sistemom Windows 10 in novejšimi napravami v storitvi Intune</span><span class="sxs-lookup"><span data-stu-id="effb2-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="effb2-109">Uvoz nastavitev omrežja Wi-Fi za naprave s sistemom Windows v storitvi Intune</span><span class="sxs-lookup"><span data-stu-id="effb2-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="effb2-110">**Pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="effb2-110">**Common Issues**</span></span>

<span data-ttu-id="effb2-111">**Uvajam profil Wi-Fi, ki je odvisen od uvedenega potrdila, določenega v profilu Wi-Fi. Vendar pa konfiguracijski profili prikazujejo stanje napake.**</span><span class="sxs-lookup"><span data-stu-id="effb2-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="effb2-112">Preverite, ali je naprava prejela potrdilo.</span><span class="sxs-lookup"><span data-stu-id="effb2-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="effb2-113">V intunu pojdite na **Vse naprave in** izberite > **napravo**.</span><span class="sxs-lookup"><span data-stu-id="effb2-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="effb2-114">Preverite, ali so navedeni vsi pričakovani profili in v uspešnem stanju.</span><span class="sxs-lookup"><span data-stu-id="effb2-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="effb2-115">Če imate za profil androida vmesna potrdila v verigi potrdil, se prepričajte, da so uvedena v napravah Android.</span><span class="sxs-lookup"><span data-stu-id="effb2-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="effb2-116">Če želite preveriti stanje potrdila, pojdite na **Konfiguracija**  >  **naprave Profili**  >  **Posrednik zaupanja vrednega potrdila o pristnosti s sistemom**  >  **Properties**  >  **Android**.</span><span class="sxs-lookup"><span data-stu-id="effb2-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="effb2-117">Če še vedno vidite napake, preglejte razdelke s postopki in odpravljanje težav.</span><span class="sxs-lookup"><span data-stu-id="effb2-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="effb2-118">Če želite več informacij, [glejte Pregled za odpravljanje težav s certifikatnimi profili SCEP z MicrosoftOm Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="effb2-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="effb2-119">**V napravo sem poslal profil Wi-Fi. Intune kaže, da je bila uspešna, vendar naprava ne vzpostavlja povezave z omrežjem Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="effb2-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="effb2-120">Uspešno stanje pomeni, da je Intune uspešno uvedel profil kot konfiguriran.</span><span class="sxs-lookup"><span data-stu-id="effb2-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="effb2-121">Vendar pa te konfiguracije morda ne ustrezajo vašim zahtevam za omrežje in/ali preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="effb2-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="effb2-122">Če želite več podrobnosti o poskusu povezave, preglejte dnevnike v infrastrukturi in storitvi za preverjanje pristnosti (v krmilniku dostopne točke Wi-Fi in strežniku NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="effb2-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="effb2-123">Če želite zbirati in pregledovati dnevnike, boste morda morali sodelovati z ekipo za omrežno infrastrukturo ali drugim prodajalcem wi-fi.</span><span class="sxs-lookup"><span data-stu-id="effb2-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>