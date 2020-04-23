---
title: Fix 0x8004de40 napaka v storitvi OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716044"
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