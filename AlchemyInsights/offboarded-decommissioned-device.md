---
title: Težave z odstranjevanjem nenajavne ali izločitev naprave iz inventarja naprave
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564609"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="3f787-102">Težave z odstranjevanjem nenajavne ali izločitev naprave iz inventarja naprave</span><span class="sxs-lookup"><span data-stu-id="3f787-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="3f787-103">Microsoft Defender za končno točko trenutno ne omogoča ročnega odstranjevanja zapisa naprave za nenajavno ali izločitev naprave iz inventarja naprav.</span><span class="sxs-lookup"><span data-stu-id="3f787-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="3f787-104">Zaradi varnostnih razlogov naprava ostane na portalu kot zgodovinski zapis do 180 dni.</span><span class="sxs-lookup"><span data-stu-id="3f787-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="3f787-105">Podatki o napravi pa so purged v skladu s konfigurirano obdobjem hranjenja.</span><span class="sxs-lookup"><span data-stu-id="3f787-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="3f787-106">**Opomba:** Nenatisljena ali izločitev naprave po sedmih dneh **samodejno** preklopi na stanje »Nedejaven«.</span><span class="sxs-lookup"><span data-stu-id="3f787-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="3f787-107">Poleg tega naprave, ki niso aktivne v zadnjih 30 dneh, niso upoštevane v podatkih, ki odražajo oceno izpostavljenosti upravljanje groženj in ranljivosti v organizaciji ali Microsoftovo oceno varnosti za naprave.</span><span class="sxs-lookup"><span data-stu-id="3f787-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="3f787-108">Če še vedno ne želite videti določenih naprav v pogledu zaloge naprav, poskusite s posneti oznako naprave, da filtrirate izločitev naprave iz pogleda inventarja naprav.</span><span class="sxs-lookup"><span data-stu-id="3f787-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="3f787-109">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="3f787-109">For more information, see:</span></span>

[<span data-ttu-id="3f787-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="3f787-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="3f787-111">Ocena izpostavljenosti v upravljanje groženj in ranljivosti</span><span class="sxs-lookup"><span data-stu-id="3f787-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="3f787-112">Popravljanje neprimernih senzorjev v aplikaciji Microsoft Defender for Endpoint</span><span class="sxs-lookup"><span data-stu-id="3f787-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="3f787-113">Kako učinkovito uporabljati označevanje (1. del)</span><span class="sxs-lookup"><span data-stu-id="3f787-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="3f787-114">Kako učinkovito uporabljati označevanje (2. del)</span><span class="sxs-lookup"><span data-stu-id="3f787-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="3f787-115">Kako učinkovito uporabljati označevanje (3. del)</span><span class="sxs-lookup"><span data-stu-id="3f787-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




