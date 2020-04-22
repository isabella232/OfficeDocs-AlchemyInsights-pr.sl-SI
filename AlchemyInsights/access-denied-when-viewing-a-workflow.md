---
title: Dostop zavrnjen pri ogledu poteka dela
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687346"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Dostop zavrnjen pri ogledu poteka dela

Poteki dela SharePoint 2013, ki poskušajo poslati e-poštno sporočilo v SharePointovo skupino, lahko spodleti s sporočilom o napaki» dostop zavrnjen «, če članstvo v SharePointovi skupini ni nastavljeno na vsi.
  
 **Če želite odpraviti to težavo, naredite naslednje:**
  
 1. Dovolite vsem, da vidijo člane SharePointove skupine.
  
 2. Odstranite SharePointovo skupino iz vrstice za ali CC e-poštnega sporočila.
  
 3. Eksplicitno dodajte uporabnike v vrstico za ali CC, če vidnost članstva ni mogoče spremeniti za SharePointovo skupino.
  
Če si želite ogledati več podrobnosti, glejte [http nepooblaščeno, da/_vti_bin/Client.SVC/SP.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  