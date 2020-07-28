---
title: Odstranjevanje podatkov in brisanje naprav iz intuna
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440466"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="22f31-102">Odstranjevanje podatkov in brisanje naprav iz intuna</span><span class="sxs-lookup"><span data-stu-id="22f31-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="22f31-103">Dejanja »Upokojijo naprave« in »Device Wipe« lahko odstranite podatke podjetja, ki jih upravlja Intune, ali pa izvedete tovarniško ponastavitev in napravo vrnete na privzete nastavitve.</span><span class="sxs-lookup"><span data-stu-id="22f31-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="22f31-104">Vpišite se v upravljanje naprav v storitvi Microsoft 365 in odi¹tejejte **aplikacije**  >  **Vse naprave**.</span><span class="sxs-lookup"><span data-stu-id="22f31-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="22f31-105">Izberite napravo, ki jo želite izbrisati.</span><span class="sxs-lookup"><span data-stu-id="22f31-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="22f31-106">Izberite vrsto oddaljenega brisa, ki ga želite narediti.</span><span class="sxs-lookup"><span data-stu-id="22f31-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="22f31-107">Upokojiti izbriše samo organizacijske informacije, medtem ko polni robčki obnovite napravo na tovarniške nastavitve.</span><span class="sxs-lookup"><span data-stu-id="22f31-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="22f31-108">Izberite **Da,** da potrdite.</span><span class="sxs-lookup"><span data-stu-id="22f31-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="22f31-109">Dokler se robček ne konča, je stanje dejanja naprave prikazano kot »V teku«.</span><span class="sxs-lookup"><span data-stu-id="22f31-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="22f31-110">Ko je dejanje dokončano, na seznamu upravljane naprave ne boste več videli mobilne naprave.</span><span class="sxs-lookup"><span data-stu-id="22f31-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="22f31-111">\*\* Opomba\*\* Podatkov podjetja ni mogoče odstraniti iz naprav, ki so pridružene Azure AD.</span><span class="sxs-lookup"><span data-stu-id="22f31-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="22f31-112">Za vse podrobnosti o učinku dejanj »Upokojii« in »Obriši«, vključno s tem, kaj se ohrani in kaj se izbriše, glejte Odstranjevanje naprav [z brisanjem, upokojitvijo ali ročnim odvijanjem naprave](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="22f31-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="22f31-113">Če želite izbrisati vse podatke iz naprave macOS, [glejte Brisanje vseh podatkov iz naprave macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="22f31-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>