---
title: 0x8004de40 pri zagonu storitve OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813668"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 pri zagonu storitve OneDrive

Če se pri prijavi v **OneDrive 0x8004de40** prikaže sporočilo o napaki, znova zaženite računalnik, ko imate vzpostavljeno povezavo s službeno ali šolsko domeno. Če po vnovičnem zagonu računalnika prejmete to napako, poskusite to, ko ste povezani s službeno ali šolsko domeno:

1. Kliknite Start in v iskalno polje vnesite **cmd** ali **ukazni** poziv, z desno tipko miške kliknite aplikacijo ukaznega poziva in izberite **Zaženi kot skrbnik.** Če ste pozvani k vnosu skrbniškega gesla ali potrditvi, vnesite geslo ali kliknite **Dovoli.**  

2. V okno ukaznega poziva vnesite **dsregcmd /leave**  in počakajte, da se ukaz dokonča. Nato vnesite **dsregcmd /join in** počakajte, da se ukaz dokonča.
3. Znova zaženite računalnik.
