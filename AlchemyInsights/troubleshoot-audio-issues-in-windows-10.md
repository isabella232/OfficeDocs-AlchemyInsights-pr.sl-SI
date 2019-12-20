---
title: Odpravljanje težav z zvočnimi težavami v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796379"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="cf119-102">Odpravljanje težav z zvokom v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="cf119-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="cf119-103">**Zaženite orodje za odpravljanje težav z zvokom**</span><span class="sxs-lookup"><span data-stu-id="cf119-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="cf119-104">Orodje za odpravljanje težav z zvokom lahko samodejno popravi težave z zvokom:</span><span class="sxs-lookup"><span data-stu-id="cf119-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="cf119-105">Izberite **Start**, vnesite **Odpravljanje težav**in nato na seznamu rezultatov izberite **Odpravljanje težav** .</span><span class="sxs-lookup"><span data-stu-id="cf119-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="cf119-106">Izberite **predvajanje zvoka** > **zaženite orodje za odpravljanje težav**.</span><span class="sxs-lookup"><span data-stu-id="cf119-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="cf119-107">**Preverite kable, glasnost, zvočnike in slušalke**</span><span class="sxs-lookup"><span data-stu-id="cf119-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="cf119-108">Preverite povezave zvočnikov in slušalk za ohlapne kable in se prepričajte, da so priključeni na pravilen priključek.</span><span class="sxs-lookup"><span data-stu-id="cf119-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="cf119-109">Preverite raven moči in glasnosti ter poskusite obračanje vseh kontrolnikov glasnosti.</span><span class="sxs-lookup"><span data-stu-id="cf119-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="cf119-110">Nekateri zvočniki in aplikacije imajo svoje kontrolnike za glasnost in morda boste morali preveriti vse, da se prepričate, ali so na pravem nivoju.</span><span class="sxs-lookup"><span data-stu-id="cf119-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="cf119-111">Poskusite vzpostaviti povezavo z drugim vrati USB.</span><span class="sxs-lookup"><span data-stu-id="cf119-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="cf119-112">**Opomba:** Ne pozabite, da zvočniki morda ne bodo delovale, ko so slušalke priključene.</span><span class="sxs-lookup"><span data-stu-id="cf119-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="cf119-113">**Preverjanje upravitelja naprav**</span><span class="sxs-lookup"><span data-stu-id="cf119-113">**Check Device Manager**</span></span>

<span data-ttu-id="cf119-114">Če želite zagotoviti, da so vozniki posodobljeni:</span><span class="sxs-lookup"><span data-stu-id="cf119-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="cf119-115">Izberite **Start**, vnesite **upravitelj naprav**in nato na seznamu rezultatov izberite **upravitelj naprav** .</span><span class="sxs-lookup"><span data-stu-id="cf119-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="cf119-116">Pod **Krmilniki za zvok, video in igre**izberite zvočno kartico, jo odprite, izberite zavihek **gonilnik** in izberite **Posodobi gonilnik**.</span><span class="sxs-lookup"><span data-stu-id="cf119-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="cf119-117">**Opomba:** Če Windows ne najde novega gonilnika, ga poiščite na spletnem mestu izdelovalca naprave in upoštevajte njihova navodila.</span><span class="sxs-lookup"><span data-stu-id="cf119-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="cf119-118">**Vnovična namestitev gonilnika**</span><span class="sxs-lookup"><span data-stu-id="cf119-118">**Reinstall the driver**</span></span>

<span data-ttu-id="cf119-119">Če ne morete posodobiti prek upravitelja naprav ali najti novega gonilnika na spletnem mestu izdelovalca, poskusite te korake:</span><span class="sxs-lookup"><span data-stu-id="cf119-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="cf119-120">V upravitelju naprav z desno miškino tipko kliknite (ali pritisnite in pridržite) zvočni gonilnik in izberite **Odstrani**.</span><span class="sxs-lookup"><span data-stu-id="cf119-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="cf119-121">Znova zaženite napravo in Windows bo poskušal znova namestiti gonilnik.</span><span class="sxs-lookup"><span data-stu-id="cf119-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="cf119-122">Če vnovična namestitev gonilnika ne deluje, poskusite uporabiti splošen zvočni gonilnik, ki je priložen sistemu Windows.</span><span class="sxs-lookup"><span data-stu-id="cf119-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="cf119-123">V upravitelju naprav z desno tipko miške kliknite (ali pritisnite in pridržite) vaš zvočni gonilnik **> posodobitev gonilnika programske opreme** > **brskajte po mojem računalniku za programsko opremo** > gonilnika, da izberem**s seznama gonilnikov naprav v računalniku**, izberite **visokoločljivostno zvočno napravo**, izberite **naprej**in sledite navodilom za namestitev.</span><span class="sxs-lookup"><span data-stu-id="cf119-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="cf119-124">**Nastavitev privzete naprave**</span><span class="sxs-lookup"><span data-stu-id="cf119-124">**Set the default device**</span></span>

<span data-ttu-id="cf119-125">Če vzpostavljate povezavo z zvočno napravo prek USB-a ali HDMI-a, boste morda morali to napravo nastaviti kot privzetega:</span><span class="sxs-lookup"><span data-stu-id="cf119-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="cf119-126">Izberite **Start**, vnesite **zvok**in nato na seznamu rezultatov izberite **zvok** ali **spremenite zvoke sistema** .</span><span class="sxs-lookup"><span data-stu-id="cf119-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="cf119-127">Na zavihku **predvajanje** izberite napravo, izberite **Nastavi privzeto**in izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="cf119-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

