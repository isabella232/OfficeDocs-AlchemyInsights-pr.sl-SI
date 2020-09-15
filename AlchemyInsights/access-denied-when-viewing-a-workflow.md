---
title: Dostop zavrnjen med ogledovanjem poteka dela
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688818"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Dostop zavrnjen med ogledovanjem poteka dela

Poteki dela programa SharePoint 2013, ki poskušajo poslati e-poštno sporočilo v SharePointovo skupino, ne morejo narediti sporočila o napaki» dostop zavrnjen «, če članstvo v SharePointovi skupini ni nastavljeno na» vsi «.
  
 **Če želite odpraviti to težavo, naredite te korake:**
  
 1. Dovolite vsem, da si ogledajo člane SharePointove skupine.
  
 2. Odstranite SharePointovo skupino iz vrstice» za «ali» Kp «v e-poštnem sporočilu.
  
 3. Eksplicitno Dodajanje uporabnikov v vrstico» za «ali» Kp «, če vidnost članstva ni mogoče spremeniti za SharePointovo skupino.
  
Če si želite ogledati več podrobnosti, se obrnite na [http nepooblaščeno za/_vti_bin/Client.SVC/SP.utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  