---
title: Nastavitve zagona v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828168"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="84c5a-102">Nastavitve zagona v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="84c5a-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="84c5a-103">**Spreminjanje, katere aplikacije se samodejno zaženejo ob zagonu**</span><span class="sxs-lookup"><span data-stu-id="84c5a-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="84c5a-104">Odprite Nastavitve [in >, > zagonu.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="84c5a-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="84c5a-105">Prepričajte se, da je kateri koli program, ki ga želite zagnati ob zagonu, **vklopljen.**</span><span class="sxs-lookup"><span data-stu-id="84c5a-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="84c5a-106">**Dodajanje programa za samodejni zagon ob zagonu**</span><span class="sxs-lookup"><span data-stu-id="84c5a-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="84c5a-107">Kliknite ali tapnite **Začetni meni** in poiščite aplikacijo, ki jo želite zagnati ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="84c5a-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="84c5a-108">Z desno tipko miške kliknite program, **kliknite Več** in nato Odpri **mesto datoteke.**</span><span class="sxs-lookup"><span data-stu-id="84c5a-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="84c5a-109">S tem odprete mesto, kjer je shranjena bližnjica do aplikacije.</span><span class="sxs-lookup"><span data-stu-id="84c5a-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="84c5a-110">Če možnost Odpri mesto datoteke ni na voljo, to pomeni, da se program ne more zagnati ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="84c5a-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="84c5a-111">Ko je mesto datoteke odprto, pritisnite tipko **z logotipom sistema Windows + R**, vnesite **shell:startup**, nato pa kliknite V **redu**.</span><span class="sxs-lookup"><span data-stu-id="84c5a-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="84c5a-112">S tem odprete mapo Zagon.</span><span class="sxs-lookup"><span data-stu-id="84c5a-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="84c5a-113">Kopirajte in prilepite bližnjico do programa z mesta datoteke v zagonsko mapo.</span><span class="sxs-lookup"><span data-stu-id="84c5a-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="84c5a-114">**Dodatne možnosti zagona (vključno z varnim načinom, nastavitvami UEFI in zagonom iz druge naprave)**</span><span class="sxs-lookup"><span data-stu-id="84c5a-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="84c5a-115">Shranite svoje delo in zaprite vse odprte dokumente, saj boste s temi koraki znova zagnali računalnik.</span><span class="sxs-lookup"><span data-stu-id="84c5a-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="84c5a-116">Pojdite na [Nastavitve in > Posodobite & obnovitev > varnost.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="84c5a-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="84c5a-117">V **razdelku Napredni zagon** kliknite Znova **zaženi** zdaj.</span><span class="sxs-lookup"><span data-stu-id="84c5a-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="84c5a-118">Ko se računalnik znova zažene, se prikaže zaslon za izbiro možnosti:</span><span class="sxs-lookup"><span data-stu-id="84c5a-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="84c5a-119">Če se želite zagnati iz naprave, kot je pogon USB, **kliknite Uporabi napravo**.</span><span class="sxs-lookup"><span data-stu-id="84c5a-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="84c5a-120">Če želite vnesti nastavitve UEFI (imenujemo jih tudi namestitev SETUP) > Dodatne možnosti **> nastavitvah vdelane programske opreme UEFI**.</span><span class="sxs-lookup"><span data-stu-id="84c5a-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="84c5a-121">Če želite vnesti varni način ali spremeniti dodatne nastavitve zagona, **> Dodatne možnosti > zagona**, nato pa kliknite Znova **zaženi.**</span><span class="sxs-lookup"><span data-stu-id="84c5a-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="84c5a-122">Morda boste morali vnesti obnovitveni [ključ za BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="84c5a-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="84c5a-123">Ko se računalnik znova zažene, kliknite nastavitev zagona, ki jo želite uporabiti.</span><span class="sxs-lookup"><span data-stu-id="84c5a-123">After your PC restarts again, click the startup setting you want to use.</span></span>