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
ms.openlocfilehash: 358bb6aa0420a845e51e0b75049c2ae790daf3690e5cfb115b234d82a29e93a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966125"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a>V portalu manjkajo naprave upravitelja konfiguracije

Za delovanje sinhronizacije naprav morajo biti [zahtevane končne točke interneta](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) dosegljive s strežnika na mestu uporabe, ki gosti vlogo stične točke storitve. Če želite odpraviti težaves s sinhronizacijo naprav, si oglejte dnevnik **CMGatewaySyncUploadWorker.log**, ki je v stični točki storitve.

Preberite več o tem, kako [pripeti najemnika k programu Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).
