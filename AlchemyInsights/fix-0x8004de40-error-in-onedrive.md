---
title: Pritrditi zmota 0x8004de40 v OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133992"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Pritrditi zmota 0x8004de40 v OneDrive

Če prejmete napako 0x8004de40 z OneDrive:

- Odmevajoč vplivati računalo, medtem ko povezan z domeno dejvaen imenik.
- Če odmevajoč ne popraviti izdaja, ločiti in ponovno napravi iz sinje AD. 

**Opomba**: Bodite v omrežju podjetja med izvajanjem teh korakov. Ne izvede te korake, ko niste mogli vzpostaviti osrednjo infrastrukturo (na primer med potovanjem). 

- Plan visok zapoved uren. 
- Razkleniti visok zapoved uren, kliknite - **Start**, desno tipko miške kliknite **ukazni poziv**in nato kliknite **Zaženi kot skrbnik**.
- Vrsto *dsregcmd /leave* in pritisnite **Enter**.
- Ko končate, vnesite *dsregcmd/JOIN* in pritisnite **Enter**.
- Ko končate, zaprite ukazni poziv.
- Odmevajoč računalo, ter poleno v OneDrive.