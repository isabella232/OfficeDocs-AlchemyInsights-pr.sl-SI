---
title: Fix 0x8004de40 napaka v storitvi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 48b29f57763ca22a71a23b2afddcac0e8e8a95db
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052053"
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