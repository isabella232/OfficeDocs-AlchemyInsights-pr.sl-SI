---
title: Nastavitve zagona v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751151"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="fe70c-102">Nastavitve zagona v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="fe70c-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="fe70c-103">**Spreminjanje, kateri programi se zaženejo samodejno ob zagonu**</span><span class="sxs-lookup"><span data-stu-id="fe70c-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="fe70c-104">Pojdite v razdelek [nastavitve > aplikacije > zagon](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="fe70c-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="fe70c-105">Preverite, ali je vklopljen kateri koli program, ki ga želite zagnati ob **zagonu.**</span><span class="sxs-lookup"><span data-stu-id="fe70c-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="fe70c-106">**Dodajanje programa za samodejno izvajanje ob zagonu**</span><span class="sxs-lookup"><span data-stu-id="fe70c-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="fe70c-107">Kliknite ali tapnite **Start** in poiščite aplikacijo, ki jo želite zagnati ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="fe70c-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="fe70c-108">Z desno tipko miške kliknite program, kliknite **več**in nato kliknite **Odpri mesto datoteke**.</span><span class="sxs-lookup"><span data-stu-id="fe70c-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="fe70c-109">Odpre se mesto, kjer je shranjena Bližnjica do programa.</span><span class="sxs-lookup"><span data-stu-id="fe70c-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="fe70c-110">Če ni možnosti za odpiranje mesta datoteke, to pomeni, da se aplikacija ne more zagnati ob zagonu.</span><span class="sxs-lookup"><span data-stu-id="fe70c-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="fe70c-111">Ko je mesto datoteke odprto, pritisnite **tipko z logotipom sistema Windows + R**, vnesite **Shell: zagon**in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="fe70c-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="fe70c-112">Odpre se zagonska mapa.</span><span class="sxs-lookup"><span data-stu-id="fe70c-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="fe70c-113">Kopirajte in prilepite bližnjico do programa iz mesta datoteke v zagonsko mapo.</span><span class="sxs-lookup"><span data-stu-id="fe70c-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="fe70c-114">**Napredne možnosti zagona (vključno z varnim načinom, nastavitvami UEFI in zagon iz druge naprave)**</span><span class="sxs-lookup"><span data-stu-id="fe70c-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="fe70c-115">Shranite delo in zaprite vse odprte dokumente, ker bodo ti koraki znova zagnali računalnik.</span><span class="sxs-lookup"><span data-stu-id="fe70c-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="fe70c-116">Pojdite na [nastavitve > posodobitev & varnost > obnovitvijo](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="fe70c-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="fe70c-117">V razdelku **napredni zagon**kliknite **znova Zaženi zdaj**.</span><span class="sxs-lookup"><span data-stu-id="fe70c-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="fe70c-118">Ko se računalnik znova zažene na zaslonu izberite možnost:</span><span class="sxs-lookup"><span data-stu-id="fe70c-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="fe70c-119">Če želite zagnati iz naprave, kot je pogon USB, kliknite **uporabi napravo**.</span><span class="sxs-lookup"><span data-stu-id="fe70c-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="fe70c-120">Če želite vnesti nastavitve UEFI (včasih se imenuje nastavitev BIOS-a), kliknite **Odpravljanje težav > napredne možnosti > nastavitve vdelane programske opreme UEFI**.</span><span class="sxs-lookup"><span data-stu-id="fe70c-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="fe70c-121">Če želite vnesti varni način ali spremeniti napredne nastavitve zagona, kliknite **Odpravljanje težav > dodatnih možnosti > nastavitve zagona**in nato **znova Zaženi**.</span><span class="sxs-lookup"><span data-stu-id="fe70c-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="fe70c-122">Morda boste pozvani k vnosu [obnovitvenega ključa za BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="fe70c-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="fe70c-123">Ko se računalnik znova zažene, kliknite nastavitev zagona, ki jo želite uporabiti.</span><span class="sxs-lookup"><span data-stu-id="fe70c-123">After your PC restarts again, click the startup setting you want to use.</span></span>