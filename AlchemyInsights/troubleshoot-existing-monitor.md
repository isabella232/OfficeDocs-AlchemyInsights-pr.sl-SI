---
title: Odpravljanje težav z obstoječim monitorjem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738584"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="dc640-102">Odpravljanje težav z obstoječim monitorjem</span><span class="sxs-lookup"><span data-stu-id="dc640-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="dc640-103">Poskusite te rešitve za odpravljanje težav z monitorjem.</span><span class="sxs-lookup"><span data-stu-id="dc640-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="dc640-104">**Osvežite zaslon monitorja:**</span><span class="sxs-lookup"><span data-stu-id="dc640-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="dc640-105">Istočasno pritisnite naslednje tipke: Windows Key + CTRL + SHIFT + B. S tem boste osvežili komunikacijo z grafičnim gonilnikom.</span><span class="sxs-lookup"><span data-stu-id="dc640-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="dc640-106">Vaši monitorji bodo utripali za trenutek in se vrnili po nekaj sekundah.</span><span class="sxs-lookup"><span data-stu-id="dc640-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="dc640-107">**Odpravljanje težav s strojno opremo monitorja:**</span><span class="sxs-lookup"><span data-stu-id="dc640-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="dc640-108">Izključite kabel, ki povezuje računalnik z monitorjem, in ga priključite nazaj.</span><span class="sxs-lookup"><span data-stu-id="dc640-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="dc640-109">Odklopite vse nebistvene naprave iz računalnika (kot so adapterji ali doki).</span><span class="sxs-lookup"><span data-stu-id="dc640-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="dc640-110">**Če ste pred kratkim namestili posodobitev v računalniku, lahko znova namestite gonilnik zaslona:**</span><span class="sxs-lookup"><span data-stu-id="dc640-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="dc640-111">Izberite **Start**, vnesite **upravitelj naprav**in izberite **upravitelj naprav** iz rezultatov.</span><span class="sxs-lookup"><span data-stu-id="dc640-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="dc640-112">Razširite razdelek **grafične kartice** , z desno miškino tipko kliknite prikazno kartico, finim izberite **lastnosti**.</span><span class="sxs-lookup"><span data-stu-id="dc640-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="dc640-113">Pomaknite se na zavihek **gonilnik** in izberite **Roll Back Driver**.</span><span class="sxs-lookup"><span data-stu-id="dc640-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="dc640-114">Opomba: če to ni na voljo ali je siva barva, izberite **ne** iz spodnjih možnosti, da se premaknete na naslednji korak.</span><span class="sxs-lookup"><span data-stu-id="dc640-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="dc640-115">Morda boste morali znova zagnati računalnik, preden bo ta sprememba učinkovali.</span><span class="sxs-lookup"><span data-stu-id="dc640-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="dc640-116">**Odstranite in znova namestite gonilnik zaslona:**</span><span class="sxs-lookup"><span data-stu-id="dc640-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="dc640-117">Izberite **Start**, vnesite **upravitelj naprav**in izberite **upravitelj naprav** iz rezultatov.</span><span class="sxs-lookup"><span data-stu-id="dc640-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="dc640-118">Razširite razdelek **prikazni vmesniki** , z desno miškino tipko kliknite prikazno kartico, finim izberite **Odstrani napravo**.</span><span class="sxs-lookup"><span data-stu-id="dc640-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="dc640-119">Izberite polje poleg možnosti **Izbriši programsko opremo gonilnika za to napravo** in izberite **Odstrani**.</span><span class="sxs-lookup"><span data-stu-id="dc640-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="dc640-120">Opomba: morda boste morali znova zagnati računalnik v tej fazi.</span><span class="sxs-lookup"><span data-stu-id="dc640-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="dc640-121">Pred vnovičnim zagonom morate zapisati preostala navodila.</span><span class="sxs-lookup"><span data-stu-id="dc640-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="dc640-122">Znova odprite upravitelja naprav.</span><span class="sxs-lookup"><span data-stu-id="dc640-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="dc640-123">Razširite razdelek **prikazni vmesniki** , z desno miškino tipko kliknite zaslonno kartico in izberite **Posodobi gonilnik**.</span><span class="sxs-lookup"><span data-stu-id="dc640-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="dc640-124">Izberite **samodejno iskanje za posodobitev programske opreme gonilnika** in sledite navodilom za namestitev.</span><span class="sxs-lookup"><span data-stu-id="dc640-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>