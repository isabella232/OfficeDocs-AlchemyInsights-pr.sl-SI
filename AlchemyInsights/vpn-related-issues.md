---
title: Težave, povezane z omrežjem VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555745"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="181dd-102">Težave, povezane z omrežjem VPN</span><span class="sxs-lookup"><span data-stu-id="181dd-102">VPN related issues</span></span>

<span data-ttu-id="181dd-103">Uspešna implementacija povezljivosti VPN za odjemalce MDM je odvisna od razporejenega profila, ki pravilno odraža zahteve infrastrukture VPN.</span><span class="sxs-lookup"><span data-stu-id="181dd-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="181dd-104">Za ustrezne nastavitve odjemalskih platform, ki jih preiskujete, glejte:</span><span class="sxs-lookup"><span data-stu-id="181dd-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="181dd-105">Nastavitve holografske naprave za Windows 10 in Windows za dodajanje povezav VPN s storitvijo Intune</span><span class="sxs-lookup"><span data-stu-id="181dd-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="181dd-106">Dodajanje nastavitev VPN v napravah s sistemom iOS in iPadOS v storitvi Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="181dd-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="181dd-107">Nastavitve naprave Android za konfiguracijo VPN v intune</span><span class="sxs-lookup"><span data-stu-id="181dd-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="181dd-108">Dodajanje nastavitev VPN v napravah macOS v programu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="181dd-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="181dd-109">Če vaš profil VPN uporablja preverjanje pristnosti na podlagi potrdila, preverite, ali so korenski certifikat in profili potrdila za preverjanje pristnosti odjemalca, povezani s profilom VPN, uspešno uvedeni.</span><span class="sxs-lookup"><span data-stu-id="181dd-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="181dd-110">**Pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="181dd-110">**Common Issues**</span></span>

<span data-ttu-id="181dd-111">**V napravo sem poslal profil VPN. Intune kaže, da je bila uspešna, vendar naprava ne vzpostavlja povezave z VPN.**</span><span class="sxs-lookup"><span data-stu-id="181dd-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="181dd-112">Uspešno stanje pomeni, da je Intune uspešno uvedel profil kot konfiguriran.</span><span class="sxs-lookup"><span data-stu-id="181dd-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="181dd-113">Vendar pa te konfiguracije morda ne ustrezajo vašim zahtevam za omrežje in/ali preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="181dd-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="181dd-114">Če želite več podrobnosti o poskusu povezave, preglejte dnevnike v infrastrukturi in storitvi za preverjanje pristnosti (v strežniku VPN in strežniku NPS/Radius).</span><span class="sxs-lookup"><span data-stu-id="181dd-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="181dd-115">Če želite zbirati in pregledovati dnevnike, boste morda morali sodelovati z ekipo za omrežno infrastrukturo ali prodajalcem vpn drugega ponudnika.</span><span class="sxs-lookup"><span data-stu-id="181dd-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="181dd-116">**Ko konfiguriram VPN po meri za iOS, funkcija VPN po aplikaciji ni na voljo.**</span><span class="sxs-lookup"><span data-stu-id="181dd-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="181dd-117">VPN za aplikacije v omrežju iOS v intunu je trenutno na voljo na določenem seznamu ponudnikov in partnerjev, ki morajo izpolnjevati tudi zahteve certifikata, preden konfigurirajo VPN za per-app.</span><span class="sxs-lookup"><span data-stu-id="181dd-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="181dd-118">Če želite več informacij, [glejte Nastavitev navideznega zasebnega omrežja za aplikacijo (VPN) za naprave s sistemom iOS/iPadOS v intunu](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="181dd-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="181dd-119">Če želite več informacij o vseh vrstah povezav VPN v intunu, glejte [Ustvarjanje profilov VPN za povezavo s strežniki VPN v intunu](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="181dd-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="181dd-120">**VPN za iOS On-Demand se ne sproži, ko je dostopan do konfigurirane domene**</span><span class="sxs-lookup"><span data-stu-id="181dd-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="181dd-121">Če želite preskusiti samodejne nastavitve VPN, nastavite te vrednosti:</span><span class="sxs-lookup"><span data-stu-id="181dd-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="181dd-122">Želim narediti to: Ovrednotiti **vsak poskus povezave**</span><span class="sxs-lookup"><span data-stu-id="181dd-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="181dd-123">Izberite, ali želite vzpostaviti **povezavo: po potrebi vzpostavite povezavo**</span><span class="sxs-lookup"><span data-stu-id="181dd-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="181dd-124">Ko uporabniki dostopajo do teh domen: **ciljno ime** *domene*</span><span class="sxs-lookup"><span data-stu-id="181dd-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="181dd-125">Če zgornja konfiguracija ni uspešna, dodajte naslednji element:</span><span class="sxs-lookup"><span data-stu-id="181dd-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="181dd-126">Ko ta URL ni dosegljiv, vsili povezavo VPN: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="181dd-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>