---
title: Fix 0x8004de40 napaka v storitvi OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755864"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 napaka v storitvi OneDrive

Če prejmete napako 0x8004de40 s storitvijo OneDrive:

- Znova zaženite prizadeti računalnik, medtem ko ste povezani z domeno Acitve Directory.
- Če vnovični zagon ne popravi težave, se Razdruži in znova pridruži napravi iz Azure AD. 

**Opomba**: med izvajanjem teh korakov morate biti v omrežju podjetja. Ne izvajajte teh korakov, ko se ne morete povezati z infrastrukturo podjetja (na primer med potovanjem). 

- Odprite visok ukazni poziv. 
- Če želite odpreti visok ukazni poziv, kliknite **Start**, z desno tipko miške kliknite **ukazni poziv**in nato kliknite **Zaženi kot skrbnik**.
- Vnesite *dsregcmd/Leave* in pritisnite **Enter**.
- Čas celoten, stavek *dsregcmd/združiti* ter časnikarstvo **nastopiti**.
- Ko končate, zaprite ukazni poziv.
- Znova zaženite računalnik in se prijavite v OneDrive.