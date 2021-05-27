---
title: Stanje senzorja za preverjanje končne točke programa Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676336"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="c82c1-102">Stanje senzorja za preverjanje končne točke programa Defender</span><span class="sxs-lookup"><span data-stu-id="c82c1-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="c82c1-103">Ploščica **Naprave s težavami s senzorjem** je na nadzorni plošči Varnostne operacije.</span><span class="sxs-lookup"><span data-stu-id="c82c1-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="c82c1-104">Na tej ploščici so informacije o tem, kako posamezna naprava zagotavlja podatke senzorja in komunicira s storitvijo Defender for Endpoint Service.</span><span class="sxs-lookup"><span data-stu-id="c82c1-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="c82c1-105">Poročilo poroča, koliko naprav zahteva pozornost in vam pomaga prepoznati naprave s težavo ter odpraviti znane težave.</span><span class="sxs-lookup"><span data-stu-id="c82c1-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="c82c1-106">Dva indikatorja stanja na ploščici ponujata informacije o številu naprav, ki storitvi ne poročajo pravilno:</span><span class="sxs-lookup"><span data-stu-id="c82c1-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="c82c1-107">**Napačno konfigurirano** Naprave, ki morda delno poročajo podatke senzorja storitvi Defender for Endpoint service in lahko imajo napake pri konfiguraciji, ki jih je treba popraviti.</span><span class="sxs-lookup"><span data-stu-id="c82c1-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="c82c1-108">**Nedejaven** Naprave, ki so prenehale poročanje storitvi Defender for Endpoint Service več kot sedem dni v preteklem mesecu.</span><span class="sxs-lookup"><span data-stu-id="c82c1-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="c82c1-109">Če kliknete katero koli od skupin, vas program usmeri na seznam Naprave, filtriran glede na vaše izbire.</span><span class="sxs-lookup"><span data-stu-id="c82c1-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="c82c1-110">Na seznamu Naprave lahko filtrirate seznam stanj po tem stanju:</span><span class="sxs-lookup"><span data-stu-id="c82c1-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="c82c1-111">**Aktivno** Naprave, ki se aktivno poročajo storitvi Defender for Endpoint Service.</span><span class="sxs-lookup"><span data-stu-id="c82c1-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="c82c1-112">**Napačno konfigurirano** Naprave, ki morda delno poročajo podatke senzorja storitvi Defender for Endpoint service, vendar imajo napake pri konfiguraciji, ki jih je treba popraviti.</span><span class="sxs-lookup"><span data-stu-id="c82c1-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="c82c1-113">Napačno konfigurirane naprave lahko imajo eno ali kombinacijo teh težav:</span><span class="sxs-lookup"><span data-stu-id="c82c1-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="c82c1-114">Brez podatkov senzorja – naprave so prenehale pošiljati podatke senzorja.</span><span class="sxs-lookup"><span data-stu-id="c82c1-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="c82c1-115">Iz naprave se lahko sprožijo omejena opozorila.</span><span class="sxs-lookup"><span data-stu-id="c82c1-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="c82c1-116">Motnje komunikacije – zmožnost komunikacije z napravo je naglušna.</span><span class="sxs-lookup"><span data-stu-id="c82c1-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="c82c1-117">Pošiljanje datotek v globinsko analizo, blokiranje datotek, izoliranje naprave iz omrežja in druga dejanja, pri katerih je potrebna komunikacija z napravo, morda ne bodo delovala.</span><span class="sxs-lookup"><span data-stu-id="c82c1-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="c82c1-118">**Nedejaven** Naprave, ki so prenehale poročanje storitvi Defender for Endpoint Service.</span><span class="sxs-lookup"><span data-stu-id="c82c1-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="c82c1-119">S funkcijo za izvoz lahko prenesete celoten seznam v obliki zapisa CSV.</span><span class="sxs-lookup"><span data-stu-id="c82c1-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="c82c1-120">Če želite več informacij, glejte [Preverjanje stanja senzorjev v aplikaciji Microsoft Defender za končno točko.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="c82c1-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="c82c1-121">Če želite več informacij o tem, kaj je povzročilo nedejavnost ali napačno konfigurirano napravo, glejte Popravljanje neprimernih senzorjev v [aplikaciji Microsoft Defender za končno točko](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span><span class="sxs-lookup"><span data-stu-id="c82c1-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
