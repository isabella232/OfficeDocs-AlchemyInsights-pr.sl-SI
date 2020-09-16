---
title: Odpravljanje napake v 0x8004de40 v OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745146"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Odpravljanje napake v 0x8004de40 v OneDrive

Če prejmete sporočilo o napaki 0x8004de40 z OneDrive:

- Znova zaženite prizadeti računalnik, medtem ko imate vzpostavljeno povezavo z domeno imenika Acitve.
- Če vnovični zagon ne odpravi težave, se obrnite na napravo in se znova pridružite napravi iz storitve Azure AD. 

**Opomba**: med izvajanjem teh korakov morate biti v omrežju podjetja. Ne izvajajte teh korakov, če ne morete vzpostaviti povezave z infrastrukturo podjetja (na primer med potovanjem). 

- Odprite povišan ukazni poziv. 
- Če želite odpreti visok ukazni poziv, kliknite **Start**, z desno tipko miške kliknite **ukazni poziv**in nato kliknite **Zaženi kot skrbnik**.
- Vnesite *dsregcmd/Leave* in pritisnite tipko **Enter**.
- Ko dokončate, vnesite *dsregcmd/JOIN* in pritisnite tipko **Enter**.
- Ko končate, zaprite ukazni poziv.
- Znova zaženite računalnik in se prijavite v OneDrive.