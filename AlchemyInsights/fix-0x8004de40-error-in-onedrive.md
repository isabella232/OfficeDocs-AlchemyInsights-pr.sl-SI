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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525075"
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