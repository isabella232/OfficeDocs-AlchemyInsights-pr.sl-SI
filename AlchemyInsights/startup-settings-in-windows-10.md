---
title: Nastavitve zagona v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2020
ms.locfileid: "42409229"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="9b10d-102">Nastavitve zagona v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="9b10d-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="9b10d-103">**Spreminjanje aplikacij, ki se samodejno zaženejo ob zagonu**</span><span class="sxs-lookup"><span data-stu-id="9b10d-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="9b10d-104">Odprite [nastavitve > aplikacije > zagon](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="9b10d-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="9b10d-105">Preverite, ali je aplikacija, ki jo želite zagnati ob zagonu, **vklopljena.**</span><span class="sxs-lookup"><span data-stu-id="9b10d-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="9b10d-106">**Dodajanje aplikacije za samodejno izvajanje ob zagonu**</span><span class="sxs-lookup"><span data-stu-id="9b10d-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="9b10d-107">Kliknite ali tapnite **Začni** in poiščite aplikacijo, ki jo želite zagnati ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="9b10d-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="9b10d-108">Z desno miškino tipko kliknite aplikacijo, kliknite **več**in nato kliknite **Odpri mesto datoteke**.</span><span class="sxs-lookup"><span data-stu-id="9b10d-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="9b10d-109">S tem se odpre mesto, kjer je shranjena Bližnjica do aplikacije.</span><span class="sxs-lookup"><span data-stu-id="9b10d-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="9b10d-110">Če ni možnosti za odpiranje mesta datoteke, to pomeni, da se aplikacija ne more zagnati ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="9b10d-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="9b10d-111">Ko je mesto datoteke odprto, pritisnite **tipko z logotipom Windows + R**, vnesite **Shell: zagon**in kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="9b10d-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="9b10d-112">To odpre mapo Startup.</span><span class="sxs-lookup"><span data-stu-id="9b10d-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="9b10d-113">Kopirajte in prilepite bližnjico do aplikacije iz mesta datoteke v mapo Startup.</span><span class="sxs-lookup"><span data-stu-id="9b10d-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="9b10d-114">**Napredne možnosti zagona (vključno z varnim načinom, nastavitvami UEFI in zagonom iz druge naprave)**</span><span class="sxs-lookup"><span data-stu-id="9b10d-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="9b10d-115">Shranite svoje delo in zaprite vse odprte dokumente, saj bodo ti koraki znova zagnali računalnik.</span><span class="sxs-lookup"><span data-stu-id="9b10d-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="9b10d-116">Odprite [nastavitve > posodobitev & varnost > Recovery](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="9b10d-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="9b10d-117">Pod **naprednim zagonom**kliknite **znova Zaženi zdaj**.</span><span class="sxs-lookup"><span data-stu-id="9b10d-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="9b10d-118">Po vnovičnem zagonu računalnika na izberite zaslon z možnostmi:</span><span class="sxs-lookup"><span data-stu-id="9b10d-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="9b10d-119">Če želite zagnati napravo, kot je pogon USB, kliknite **uporabi napravo**.</span><span class="sxs-lookup"><span data-stu-id="9b10d-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="9b10d-120">Če želite vnesti nastavitve UEFI (včasih imenovane nastavitve BIOS-a), kliknite **Odpravljanje težav > napredne možnosti > nastavitve vdelane programske opreme UEFI**.</span><span class="sxs-lookup"><span data-stu-id="9b10d-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="9b10d-121">Če želite vnesti varni način ali spremeniti napredne nastavitve zagona, kliknite **Odpravljanje težav > napredne možnosti > nastavitve zagona**, nato kliknite **vnovični zagon**.</span><span class="sxs-lookup"><span data-stu-id="9b10d-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="9b10d-122">Morda boste morali vnesti [obnovitveni ključ za BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="9b10d-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="9b10d-123">Ko se računalnik znova zažene, kliknite nastavitev zagona, ki jo želite uporabiti.</span><span class="sxs-lookup"><span data-stu-id="9b10d-123">After your PC restarts again, click the startup setting you want to use.</span></span>