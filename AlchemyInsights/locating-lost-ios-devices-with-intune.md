---
title: Iskanje izgubljenih naprav s sistemom iOS z napravo Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440429"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="ece20-102">Iskanje izgubljenih naprav s sistemom iOS z napravo Intune</span><span class="sxs-lookup"><span data-stu-id="ece20-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="ece20-103">Če omogočite izgubljeni način v napravi s sistema iOS, lahko skrbnik na zaklenjenem zaslonu prikaže sporočilo in telefonsko številko stika.</span><span class="sxs-lookup"><span data-stu-id="ece20-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="ece20-104">Ko je omogočen izgubljeni način, lahko skrbnik uporabi dejanje Iskanje naprave za prepoznavanje fizične lokacije naprave.</span><span class="sxs-lookup"><span data-stu-id="ece20-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="ece20-105">Dejanje najdi napravo v intunu deluje z napravami s sistemom iOS, da prikaže lokacijo določene naprave na zemljevidu.</span><span class="sxs-lookup"><span data-stu-id="ece20-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="ece20-106">Če uporabite to dejanje, mora biti naprava s sistemom iOS v:</span><span class="sxs-lookup"><span data-stu-id="ece20-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="ece20-107">Nadzorovani način</span><span class="sxs-lookup"><span data-stu-id="ece20-107">Supervised mode</span></span>
- <span data-ttu-id="ece20-108">Izgubljeni način</span><span class="sxs-lookup"><span data-stu-id="ece20-108">Lost mode</span></span>

<span data-ttu-id="ece20-109">Če želite več informacij, [glejte Omogočanje izgubljenega načina v napravah s sistemom iOS/iPadOS z napravama Intune in Poiščite izgubljene](https://docs.microsoft.com/intune/device-lost-mode) [ali ukradene naprave iOS/iPadOS z napravami Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="ece20-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="ece20-110">**Pogosta vprašanja**</span><span class="sxs-lookup"><span data-stu-id="ece20-110">**FAQ**</span></span>

<span data-ttu-id="ece20-111">V: Izdal sem oddaljeno dejanje za odstranitev podatkov podjetja iz naprave, zdaj pa je obtičal v stanju čakanja.</span><span class="sxs-lookup"><span data-stu-id="ece20-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="ece20-112">O: Če želite, da se oddaljeno dejanje uspešno dokonča, mora biti ciljna naprava dosegljiva in zdrava.</span><span class="sxs-lookup"><span data-stu-id="ece20-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="ece20-113">V teh primerih oddaljeno dejanje ostane v stanju čakanja 30 dni ali dokler naprava ne potrdi ukaza:</span><span class="sxs-lookup"><span data-stu-id="ece20-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="ece20-114">Če naprava nima povezave</span><span class="sxs-lookup"><span data-stu-id="ece20-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="ece20-115">Ko naprava izgubi status upravljanja z napravo Intune</span><span class="sxs-lookup"><span data-stu-id="ece20-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="ece20-116">Če menite, da se naprava ne bo več prijavila in da ne bo mogla odstraniti podatkov podjetja, izberite Izbriši.</span><span class="sxs-lookup"><span data-stu-id="ece20-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="ece20-117">Če izbrišete napravo, odstranite zapis naprave, tako da ga ne bo več na seznamu naprav Intune.</span><span class="sxs-lookup"><span data-stu-id="ece20-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="ece20-118">Če naprava znova postane aktivna, jo bo moral uporabnik znova včlatiti.</span><span class="sxs-lookup"><span data-stu-id="ece20-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="ece20-119">V: Zakaj nekatera oddaljena dejanja niso na voljo za uporabo?</span><span class="sxs-lookup"><span data-stu-id="ece20-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="ece20-120">O: Vse platforme ne podpirajo vseh dejanj oddaljenih naprav.</span><span class="sxs-lookup"><span data-stu-id="ece20-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="ece20-121">Naslednja oddaljena dejanja so specifična za platformo, zato so na voljo samo za ugotovljene platforme.</span><span class="sxs-lookup"><span data-stu-id="ece20-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="ece20-122">Bypass Activation Lock (samo za iOS)</span><span class="sxs-lookup"><span data-stu-id="ece20-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="ece20-123">Nov začetek (samo windows)</span><span class="sxs-lookup"><span data-stu-id="ece20-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="ece20-124">Izgubljen način (samo za iOS)</span><span class="sxs-lookup"><span data-stu-id="ece20-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="ece20-125">Iskanje naprave (samo za iOS)</span><span class="sxs-lookup"><span data-stu-id="ece20-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="ece20-126">Vnovični zagon (samo windows)</span><span class="sxs-lookup"><span data-stu-id="ece20-126">Restart (Windows only)</span></span>

<span data-ttu-id="ece20-127">Če želite več podrobnosti o vsakem dejanju, glejte Dejanja [naprave, ki so na voljo](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="ece20-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>