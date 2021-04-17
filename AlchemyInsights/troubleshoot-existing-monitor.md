---
title: Odpravljanje težav z obstoječim monitorjem
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824595"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="22c4b-102">Odpravljanje težav z obstoječim monitorjem</span><span class="sxs-lookup"><span data-stu-id="22c4b-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="22c4b-103">Poskusite s temi rešitvami odpraviti težave na monitorju.</span><span class="sxs-lookup"><span data-stu-id="22c4b-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="22c4b-104">**Osvežite zaslon monitorja:**</span><span class="sxs-lookup"><span data-stu-id="22c4b-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="22c4b-105">Hkrati pritisnite te tipke: Tipka Windows + Ctrl + Shift + B. Tako boste osvežili komunikacijo z grafičnim gonilnikom.</span><span class="sxs-lookup"><span data-stu-id="22c4b-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="22c4b-106">Zasloni bodo za trenutek utripajoči in se čez nekaj sekund vrnili.</span><span class="sxs-lookup"><span data-stu-id="22c4b-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="22c4b-107">**Odpravljanje težav s strojno opremo monitorja:**</span><span class="sxs-lookup"><span data-stu-id="22c4b-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="22c4b-108">Izključite kabel, ki povezuje računalnik z monitorjem, in ga znova priključite.</span><span class="sxs-lookup"><span data-stu-id="22c4b-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="22c4b-109">Izključite vse naprave, ki niso pomembne, z računalnikom (kot so kartice ali priklopne postaje).</span><span class="sxs-lookup"><span data-stu-id="22c4b-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="22c4b-110">**Če ste v računalnik nedavno namestili posodobitev, lahko gonilnik grafične kartice povrnite tako:**</span><span class="sxs-lookup"><span data-stu-id="22c4b-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="22c4b-111">Izberite **Začetni** meni , **vnesite upravitelja** naprav in **med rezultati** izberite Upravitelj naprav.</span><span class="sxs-lookup"><span data-stu-id="22c4b-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="22c4b-112">Razširite **razdelek Grafične kartice,** z desno tipko miške kliknite grafično kartico in izberite **Lastnosti.**</span><span class="sxs-lookup"><span data-stu-id="22c4b-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="22c4b-113">Pomaknite se na **zavihek Gonilnik** in izberite **Pomakni nazaj gonilnik**.</span><span class="sxs-lookup"><span data-stu-id="22c4b-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="22c4b-114">Opomba: Če ta možnost ni na voljo ali je zatemnjena, izberite Ne **med** spodnjimi možnostmi, da se premaknete na naslednji korak.</span><span class="sxs-lookup"><span data-stu-id="22c4b-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="22c4b-115">Preden bodo spremembe začele veljati, boste morda morali znova zagnati računalnik.</span><span class="sxs-lookup"><span data-stu-id="22c4b-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="22c4b-116">**Odstranite in znova namestite gonilnik grafične kartice:**</span><span class="sxs-lookup"><span data-stu-id="22c4b-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="22c4b-117">Izberite **Začetni** meni , **vnesite upravitelja** naprav in **med rezultati** izberite Upravitelj naprav.</span><span class="sxs-lookup"><span data-stu-id="22c4b-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="22c4b-118">Razširite **razdelek Grafične kartice,** z desno tipko miške kliknite grafično kartico in izberite **Odstrani napravo.**</span><span class="sxs-lookup"><span data-stu-id="22c4b-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="22c4b-119">Izberite polje ob možnosti Izbriši **programsko opremo gonilnika za to napravo in** izberite **Odstrani**.</span><span class="sxs-lookup"><span data-stu-id="22c4b-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="22c4b-120">Opomba: Na tej stopnji boste morda pozvani k ponovnemu zagonu računalnika.</span><span class="sxs-lookup"><span data-stu-id="22c4b-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="22c4b-121">Pred ponovnim zagonom si zapišite preostala navodila.</span><span class="sxs-lookup"><span data-stu-id="22c4b-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="22c4b-122">Znova odprite upravitelja naprav.</span><span class="sxs-lookup"><span data-stu-id="22c4b-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="22c4b-123">Razširite **razdelek Grafične kartice,** z desno tipko miške kliknite grafično kartico in izberite **Posodobi gonilnik**.</span><span class="sxs-lookup"><span data-stu-id="22c4b-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="22c4b-124">Izberite **Samodejno poišči programsko opremo za posodobitev in** upoštevajte navodila za namestitev.</span><span class="sxs-lookup"><span data-stu-id="22c4b-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>