---
title: 0x8004de40 pri zagonu OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946595"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 pri zagonu OneDrive

Če se pri prijavi v **0x8004de40** prikaže sporočilo o napaki OneDrive znova zaženite računalnik, medtem ko imate vzpostavljeno povezavo s službeno ali šolsko domeno. Če po vnovičnem zagonu računalnika prejmete to napako, poskusite to, ko ste povezani s službeno ali šolsko domeno:

1. Kliknite Start in v iskalno polje vnesite **cmd** ali **ukazni** poziv, z desno tipko miške kliknite aplikacijo ukaznega poziva in izberite **Zaženi kot skrbnik.** Če ste pozvani k vnosu skrbniškega gesla ali potrditvi, vnesite geslo ali kliknite **Dovoli.**  

2. V okno ukaznega poziva vnesite **dsregcmd /leave**  in počakajte, da se ukaz dokonča. Nato vnesite **dsregcmd /join in** počakajte, da se ukaz dokonča.
3. Znova zaženite računalnik.
