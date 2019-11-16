---
title: Dostop zavrnjen pri ogledu poteka dela
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747764"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Dostop zavrnjen pri ogledu poteka dela

Poteki dela SharePoint 2013, ki poskušajo poslati e-poštno sporočilo v SharePointovo skupino, lahko spodleti s sporočilom o napaki» dostop zavrnjen «, če članstvo v SharePointovi skupini ni nastavljeno na vsi.
  
 **Če želite odpraviti to težavo, naredite naslednje:**
  
 1. Dovolite vsem, da vidijo člane SharePointove skupine.
  
 2. Odstranite SharePointovo skupino iz vrstice za ali CC e-poštnega sporočila.
  
 3. Eksplicitno dodajte uporabnike v vrstico za ali CC, če vidnost članstva ni mogoče spremeniti za SharePointovo skupino.
  
Če si želite ogledati več podrobnosti, glejte [http nepooblaščeno, da/_vti_bin/Client.SVC/SP.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  