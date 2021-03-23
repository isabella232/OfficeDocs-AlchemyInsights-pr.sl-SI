---
title: Sprostitev prostora na pogonu v sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037949"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="49acd-102">Sprostitev prostora na pogonu v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="49acd-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="49acd-103">Na voljo sta dve možnosti za sprostitev prostora na pogonu v sistemu Windows:</span><span class="sxs-lookup"><span data-stu-id="49acd-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="49acd-104">Sprostite prostor na pogonu v sistemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="49acd-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="49acd-105">Sprostite prostor za posodobitve sistema Windows 10 z zunanjo napravo za shranjevanje.</span><span class="sxs-lookup"><span data-stu-id="49acd-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="49acd-106">Če imate še vedno nizek prostor na disku, potem ko uporabljate čiščenje diska, je mogoče, da se vaša mapa» Temp «hitro napolni z datotekami aplikacije (. APPX), ki jih uporablja Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="49acd-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="49acd-107">To težavo odpravite tako, da ponastavite shrambo, počistite predpomnilnik shrambe in nato zaženete orodje za odpravljanje težav s storitvijo Windows Update.</span><span class="sxs-lookup"><span data-stu-id="49acd-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="49acd-108">Preden nadaljujete s temi koraki, se prepričajte, da je Microsoft Store zaprt.</span><span class="sxs-lookup"><span data-stu-id="49acd-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="49acd-109">**1. korak: ponastavitev trgovine Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="49acd-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="49acd-110">**Opomba** S tem trajno izbrišete podatke programa v napravi, vključno z vašimi nastavitvami in podrobnostmi za vpis.</span><span class="sxs-lookup"><span data-stu-id="49acd-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="49acd-111">Izberite» **Start**  >  **Settings**  >  **apps**  >  **apps & funkcije**«.</span><span class="sxs-lookup"><span data-stu-id="49acd-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="49acd-112">Na seznamu aplikacij poiščite in izberite Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="49acd-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="49acd-113">Izberite **dodatne možnosti**.</span><span class="sxs-lookup"><span data-stu-id="49acd-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="49acd-114">Pomaknite se navzdol in izberite **Ponastavi**, nato pa **potrdite polje Ponastavi**.</span><span class="sxs-lookup"><span data-stu-id="49acd-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="49acd-115">**2. korak: počistite predpomnilnik trgovine Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="49acd-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="49acd-116">Pritisnite tipko z logotipom sistema Windows + R, da odprete pogovorno okno Zaženi.</span><span class="sxs-lookup"><span data-stu-id="49acd-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="49acd-117">Vnesite wsreset.exe in izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="49acd-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="49acd-118">Odpre se okno s praznim ukaznim pozivom.</span><span class="sxs-lookup"><span data-stu-id="49acd-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="49acd-119">Po približno 10 sekundah se okno zapre in trgovina se odpre samodejno.</span><span class="sxs-lookup"><span data-stu-id="49acd-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="49acd-120">**3. korak: ponastavitev sistema Windows Update**</span><span class="sxs-lookup"><span data-stu-id="49acd-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="49acd-121">Izberite» **Začni**  >  posodobitve **Nastavitev «**  >  **& varnostno**  >  **Odpravljanje težav**.</span><span class="sxs-lookup"><span data-stu-id="49acd-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="49acd-122">Pomaknite se navzdol in izberite **Windows Update** s seznama, nato pa izberite **Zaženi orodje za odpravljanje težav**.</span><span class="sxs-lookup"><span data-stu-id="49acd-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="49acd-123">Znova zaženite računalnik in preverite, ali še vedno prihaja do težave.</span><span class="sxs-lookup"><span data-stu-id="49acd-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

