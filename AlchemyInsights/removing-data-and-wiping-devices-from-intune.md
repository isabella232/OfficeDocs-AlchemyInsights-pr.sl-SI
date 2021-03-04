---
title: Odstranjevanje podatkov in počistite napravo iz Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416329"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="0d933-102">Odstranjevanje podatkov in počistite napravo iz Intune</span><span class="sxs-lookup"><span data-stu-id="0d933-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="0d933-103">Oddaljena dejanja Ukinitev naprave in Brisanje podatkov iz naprave lahko uporabite za odstranitev podatkov podjetja, ki jih upravlja Intune, ali za ponastavitev na tovarniške nastavitve in vrnitev naprave na privzete nastavitve.</span><span class="sxs-lookup"><span data-stu-id="0d933-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="0d933-104">Prijavite se v Upravljanje naprav okolja Microsoft 365 in pojdite na **Naprave** > **Vse naprave**.</span><span class="sxs-lookup"><span data-stu-id="0d933-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="0d933-105">Izberite napravo, ki jo želite počistiti.</span><span class="sxs-lookup"><span data-stu-id="0d933-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="0d933-106">Izberite vrsto oddaljenega brisanja, ki ga želite izvesti.</span><span class="sxs-lookup"><span data-stu-id="0d933-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="0d933-107">Ukinitev izbriše samo organizacijske podatke, popolno brisanje podatkov iz naprave pa obnovi tovarniške nastavitve naprave.</span><span class="sxs-lookup"><span data-stu-id="0d933-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="0d933-108">Za potrditev kliknite **Da**.</span><span class="sxs-lookup"><span data-stu-id="0d933-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="0d933-109">Dokler se brisanje ne konča, se stanje dejanja naprave prikazuje kot *Ukinitev v čakanju*.</span><span class="sxs-lookup"><span data-stu-id="0d933-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="0d933-110">Po končanem dejanju mobilna naprava ne bo več vidna na seznamu upravljane naprave.</span><span class="sxs-lookup"><span data-stu-id="0d933-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="0d933-111">Podatkov podjetja ni mogoče odstraniti iz naprav, PRIDRUŽENIH Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0d933-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="0d933-112">Za vse podrobnosti o učinku ukrepov ukinitve in brisanja, vključno s tem, kaj se obdrži in kaj izbriše, glejte naslednjo dokumentacijo:</span><span class="sxs-lookup"><span data-stu-id="0d933-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="0d933-113">[Odstranite naprave z brisanjem, ukinitvijo ali ročnim odjavljanjem naprave](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="0d933-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="0d933-114">Kako izbrisati samo poslovne podatke iz aplikacij, ki jih upravlja Intune</span><span class="sxs-lookup"><span data-stu-id="0d933-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="0d933-115">[Izbrišite vse podatke iz naprave macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="0d933-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>