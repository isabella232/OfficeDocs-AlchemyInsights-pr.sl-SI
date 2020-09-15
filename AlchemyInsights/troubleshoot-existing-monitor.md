---
title: Odpravljanje težav z obstoječim monitorjem
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690727"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="1b889-102">Odpravljanje težav z obstoječim monitorjem</span><span class="sxs-lookup"><span data-stu-id="1b889-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="1b889-103">Poskusite odpraviti te rešitve za odpravljanje težav z monitorjem.</span><span class="sxs-lookup"><span data-stu-id="1b889-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="1b889-104">**Osvežitev zaslona monitorja:**</span><span class="sxs-lookup"><span data-stu-id="1b889-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="1b889-105">Hkrati pritisnite te tipke: tipka Windows + CTRL + SHIFT + B. S tem boste osvežili komunikacijo z grafičnim gonilnikom.</span><span class="sxs-lookup"><span data-stu-id="1b889-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="1b889-106">Monitorji bodo vsak trenutek utripali in se vrnili po nekaj sekundah.</span><span class="sxs-lookup"><span data-stu-id="1b889-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="1b889-107">**Odpravljanje težav s spremljanjem strojne opreme:**</span><span class="sxs-lookup"><span data-stu-id="1b889-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="1b889-108">Odklopite kabel s povezavo med računalnikom in monitorjem ter ga znova vključite.</span><span class="sxs-lookup"><span data-stu-id="1b889-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="1b889-109">Prekinite povezavo z vsemi nebistvenimi napravami iz računalnika (na primer adapterji ali doki).</span><span class="sxs-lookup"><span data-stu-id="1b889-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="1b889-110">**Če ste nedavno namestili posodobitev v računalnik, lahko vrnete gonilnik za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="1b889-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="1b889-111">Izberite **Start**, vnesite **upravitelj naprav**in v rezultatih izberite **upravitelj naprav** .</span><span class="sxs-lookup"><span data-stu-id="1b889-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="1b889-112">Razširite razdelek **prikaz adapterji** , z desno tipko miške kliknite zaslonsko kartico in izberite **lastnosti**.</span><span class="sxs-lookup"><span data-stu-id="1b889-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="1b889-113">Premaknite se do zavihka **gonilnik** in izberite **Prekliči gonilnik**.</span><span class="sxs-lookup"><span data-stu-id="1b889-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="1b889-114">Opomba: če ta možnost ni na voljo ali je zatemnjena, izberite **ne** iz spodnjih možnosti, da se premaknete na naslednji korak.</span><span class="sxs-lookup"><span data-stu-id="1b889-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="1b889-115">Morda boste morali znova zagnati računalnik, preden bodo spremembe začele veljati.</span><span class="sxs-lookup"><span data-stu-id="1b889-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="1b889-116">**Odstranite in znova namestite gonilnik za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="1b889-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="1b889-117">Izberite **Start**, vnesite **upravitelj naprav**in v rezultatih izberite **upravitelj naprav** .</span><span class="sxs-lookup"><span data-stu-id="1b889-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="1b889-118">Razširite razdelek **prikaz adapterji** , z desno tipko miške kliknite zaslonsko kartico in izberite **Odstrani napravo**.</span><span class="sxs-lookup"><span data-stu-id="1b889-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="1b889-119">Izberite polje ob možnosti **brisanje programske opreme gonilnika za to napravo** in izberite **Odstrani**.</span><span class="sxs-lookup"><span data-stu-id="1b889-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="1b889-120">Opomba: morda boste pozvani, da znova zaženete računalnik na tej stopnji.</span><span class="sxs-lookup"><span data-stu-id="1b889-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="1b889-121">Pred vnovičnim zagonom preglejte preostala navodila.</span><span class="sxs-lookup"><span data-stu-id="1b889-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="1b889-122">Znova odprite upravitelja naprav.</span><span class="sxs-lookup"><span data-stu-id="1b889-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="1b889-123">Razširite razdelek **prikaz kartic** , z desno tipko miške kliknite zaslonsko kartico in izberite **Posodobi gonilnik**.</span><span class="sxs-lookup"><span data-stu-id="1b889-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="1b889-124">Izberite **samodejno iskanje za posodobitev gonilnika programske opreme** in sledite navodilom za namestitev.</span><span class="sxs-lookup"><span data-stu-id="1b889-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>