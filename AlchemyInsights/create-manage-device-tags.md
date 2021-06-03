---
title: Ustvarjanje in upravljanje oznak ali skupin naprave
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731968"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="2dbaa-102">Ustvarjanje in upravljanje oznak ali skupin naprave</span><span class="sxs-lookup"><span data-stu-id="2dbaa-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="2dbaa-103">Dodajte oznake v naprave, da ustvarite logično stisko skupine.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="2dbaa-104">Oznake naprave podpirajo ustrezno preslikavo omrežja, kar vam omogoča, da priložite različne oznake, da zajamete kontekst in omogočite ustvarjanje dinamičnega seznama kot del dogodka.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="2dbaa-105">Oznake lahko uporabite kot filter v pogledu seznama Naprave ali za združevanje naprav.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="2dbaa-106">Če želite več informacij o skupinah v napravah, glejte [Ustvarjanje in upravljanje oznak naprave.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="2dbaa-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="2dbaa-107">Oznake lahko v naprave dodate tako:</span><span class="sxs-lookup"><span data-stu-id="2dbaa-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="2dbaa-108">Uporaba portala</span><span class="sxs-lookup"><span data-stu-id="2dbaa-108">Using the portal</span></span>

- <span data-ttu-id="2dbaa-109">Nastavitev vrednosti registrskega ključa</span><span class="sxs-lookup"><span data-stu-id="2dbaa-109">Setting a registry key value</span></span>
 
<span data-ttu-id="2dbaa-110">**Opomba:** Med časom, ko je oznaka dodana napravi, in njeno razpoložljivostjo na seznamu naprav in na strani naprave je lahko zakasnitev.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="2dbaa-111">Če želite dodati oznake naprave z API-jem, [glejte Dodajanje ali odstranjevanje oznak API-ja naprave.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="2dbaa-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="2dbaa-112">Dodajanje in upravljanje oznak naprave s portalom</span><span class="sxs-lookup"><span data-stu-id="2dbaa-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="2dbaa-113">Izberite napravo, v ki jo želite upravljati z oznakami.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="2dbaa-114">Napravo lahko izberete ali poiščete v katerem koli od teh pogledov:</span><span class="sxs-lookup"><span data-stu-id="2dbaa-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="2dbaa-115">**Nadzorna plošča varnostnih operacij** Izberite ime naprave v razdelku Top naprave z aktivnimi opozorili.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="2dbaa-116">**Čakalna vrsta** opozoril – V čakalni vrsti z opozorili izberite ime naprave poleg ikone naprave.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="2dbaa-117">**Seznam naprav** – na seznamu naprav izberite ime naprave.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="2dbaa-118">**Iskalno** polje – na spustnem meniju izberite Naprava in vnesite ime naprave.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="2dbaa-119">Do strani z opozorilom lahko odpreti tudi v pogledih datoteke in naslovov IP.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="2dbaa-120">V **vrstici z dejanji** odgovora izberite Upravljaj oznake.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="2dbaa-121">Vnesite, da najdete ali ustvarite oznake.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-121">Type to find or create tags.</span></span>

<span data-ttu-id="2dbaa-122">Oznake so dodane pogledu naprave in se odražajo v pogledu seznama Naprave.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="2dbaa-123">S filtrom Oznake si lahko ogledate ustrezen seznam naprav.</span><span class="sxs-lookup"><span data-stu-id="2dbaa-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="2dbaa-124">Če želite več informacij, [glejte Ustvarjanje in upravljanje oznak naprave.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="2dbaa-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>