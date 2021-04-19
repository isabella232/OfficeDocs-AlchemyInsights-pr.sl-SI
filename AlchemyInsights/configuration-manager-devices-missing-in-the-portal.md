---
title: V portalu manjkajo naprave upravitelja konfiguracije
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817260"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="76c40-102">V portalu manjkajo naprave upravitelja konfiguracije</span><span class="sxs-lookup"><span data-stu-id="76c40-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="76c40-103">Za delovanje sinhronizacije naprav morajo biti [zahtevane končne točke interneta](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) dosegljive s strežnika na mestu uporabe, ki gosti vlogo stične točke storitve.</span><span class="sxs-lookup"><span data-stu-id="76c40-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="76c40-104">Če želite odpraviti težaves s sinhronizacijo naprav, si oglejte dnevnik **CMGatewaySyncUploadWorker.log**, ki je v stični točki storitve.</span><span class="sxs-lookup"><span data-stu-id="76c40-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="76c40-105">Preberite več o tem, kako [pripeti najemnika k programu Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="76c40-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
