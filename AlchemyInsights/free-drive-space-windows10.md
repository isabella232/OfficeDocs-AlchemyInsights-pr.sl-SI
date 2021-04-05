---
title: Nekaj prostora na pogonu v sistemu Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505372"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="37663-102">Nekaj prostora na pogonu v sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="37663-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="37663-103">Nekaj možnosti za posodobitev prostora na pogonu v sistemu Windows:</span><span class="sxs-lookup"><span data-stu-id="37663-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="37663-104">V sistemu Windows 10 lahko prostor na pogonu nekaj prostora zasukate.</span><span class="sxs-lookup"><span data-stu-id="37663-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="37663-105">Z zunanjo napravo za shranjevanje lahko nekaj prostora posodobite za Windows 10.</span><span class="sxs-lookup"><span data-stu-id="37663-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="37663-106">Če je po uporabi čiščenja diska še vedno malo prostora, se lahko v mapi »Temp« hitro zapolnijo datoteke programa (.appx), ki jih uporablja Trgovina Microsoft.</span><span class="sxs-lookup"><span data-stu-id="37663-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="37663-107">Če želite odpraviti to težavo, ponastavite Trgovino, počistite predpomnilnik Trgovine in nato zaženite orodje za odpravljanje težav s storitvijo Windows Update.</span><span class="sxs-lookup"><span data-stu-id="37663-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="37663-108">Preden nadaljujete s temi koraki, se prepričajte, da je Trgovina Microsoft zaprta.</span><span class="sxs-lookup"><span data-stu-id="37663-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="37663-109">**1. korak: Ponastavite Trgovino Microsoft**</span><span class="sxs-lookup"><span data-stu-id="37663-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="37663-110">**Upoštevajte** S tem trajno izbrišete podatke programa v napravi, vključno z nastavitvami in podrobnostmi o vpisu.</span><span class="sxs-lookup"><span data-stu-id="37663-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="37663-111">Izberite **Začni** > **nastavitve** > **Programi** > **programi in funkcije, ki**.</span><span class="sxs-lookup"><span data-stu-id="37663-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="37663-112">Na seznamu aplikacij poiščite in izberite Trgovino Microsoft.</span><span class="sxs-lookup"><span data-stu-id="37663-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="37663-113">Izberite **»Dodatne možnosti**«.</span><span class="sxs-lookup"><span data-stu-id="37663-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="37663-114">Pomaknite se navzdol in izberite **Reset**(Ponastavi), nato **Confirm Reset**(Ponastavi).</span><span class="sxs-lookup"><span data-stu-id="37663-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="37663-115">**2. korak: počistite predpomnilnik Trgovine Microsoft**</span><span class="sxs-lookup"><span data-stu-id="37663-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="37663-116">Pritisnite tipko z logotipom sistema Windows+R, da odprete pogovorno okno Zaženi.</span><span class="sxs-lookup"><span data-stu-id="37663-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="37663-117">Vnesite wsreset.exe in izberite **»V**«.</span><span class="sxs-lookup"><span data-stu-id="37663-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="37663-118">Odpre se prazno okno ukaznega poziva.</span><span class="sxs-lookup"><span data-stu-id="37663-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="37663-119">Po približno 10 sekundah se okno zapre, Trgovina pa se odpre samodejno.</span><span class="sxs-lookup"><span data-stu-id="37663-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="37663-120">**3. korak: Ponastavitev storitve Windows Update**</span><span class="sxs-lookup"><span data-stu-id="37663-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="37663-121">Izberite **Začni** > **nastavitve** > **»Posodobitev in** > **odpravljanje**«.</span><span class="sxs-lookup"><span data-stu-id="37663-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="37663-122">Pomaknite se navzdol in **izberite** Windows Update in izberite **Zaženite orodje za odpravljanje**.</span><span class="sxs-lookup"><span data-stu-id="37663-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="37663-123">Znova zaženite računalnik in preverite, ali še vedno prihaja do te težave.</span><span class="sxs-lookup"><span data-stu-id="37663-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

