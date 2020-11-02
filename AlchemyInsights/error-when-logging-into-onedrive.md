---
title: 0x8004de40 Napaka pri zagonu OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823118"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 Napaka pri zagonu OneDrive

Če prejmete sporočilo o napaki **0x8004de40** pri prijavi v OneDrive, znova zaženite računalnik, medtem ko imate vzpostavljeno povezavo s službenim ali šolskim domeno. Če se po vnovičnem zagonu prikaže to sporočilo o napaki, poskusite to, medtem ko imate vzpostavljeno povezavo s službenim ali šolskim domeno:

1. Kliknite Start in vnesite **cmd** ali **ukazni poziv**  v iskalno polje, z desno tipko miške kliknite aplikacijo ukazni poziv, nato pa izberite  **Zaženi kot skrbnik** . Če ste pozvani k skrbniškemu geslu ali potrditvi, vnesite geslo ali kliknite **Dovoli** .  

2. V okno ukazni poziv vnesite **dsregcmd/Leave**  in počakajte, da se ukaz dokonča. Nato vnesite **dsregcmd/JOIN** in počakajte, da se ukaz dokonča.
3. Znova zaženite računalnik.
