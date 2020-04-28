---
title: V portalu manjkajo naprave upravitelja konfiguracije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790233"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="452e5-102">V portalu manjkajo naprave upravitelja konfiguracije</span><span class="sxs-lookup"><span data-stu-id="452e5-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="452e5-103">Za delovanje sinhronizacije naprav morajo biti [zahtevane končne točke interneta](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) dosegljive s strežnika na mestu uporabe, ki gosti vlogo stične točke storitve.</span><span class="sxs-lookup"><span data-stu-id="452e5-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="452e5-104">Če želite odpraviti težaves s sinhronizacijo naprav, si oglejte dnevnik **CMGatewaySyncUploadWorker.log**, ki je v stični točki storitve.</span><span class="sxs-lookup"><span data-stu-id="452e5-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="452e5-105">Preberite več o tem, kako [pripeti najemnika k programu Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="452e5-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
