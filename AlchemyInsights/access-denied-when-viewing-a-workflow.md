---
title: Dostop zavrnjen pri ogledu poteka dela
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955217"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Dostop zavrnjen pri ogledu poteka dela

SharePoint 2013 Poteki dela, ki poskušajo poslati e-poštno sporočilo skupini storitve SharePoint, lahko ne uspejo, pri tem pa se prikaže sporočilo o napaki »Dostop zavrnjen«, če članstvo v skupini SharePoint ni nastavljeno na Vsi.
  
 **Če želite odpraviti to težavo, naredite to:**
  
 1. Vsem dovolite, da vidijo člane SharePoint skupine.
  
 2. Odstranite skupino SharePoint iz vrstice Za ali Kp e-poštnega sporočila.
  
 3. Izrecno dodajte uporabnike v vrstico Za ali Kp, če vidljivosti članstva ni mogoče spremeniti za SharePoint skupine.
  
Če si želite ogledati več podrobnosti, [glejte HTTP Nepooblaščen dostop do strežnika /_vti_bin/client.svc/sp.utilities.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  