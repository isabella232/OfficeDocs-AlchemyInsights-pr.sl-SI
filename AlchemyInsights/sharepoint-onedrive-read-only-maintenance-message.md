---
title: Za sporočilo o vzdrževanju za branje pri poskusu uporabe storitve SharePoint ali OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051297"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Za sporočilo o vzdrževanju za branje pri poskusu uporabe storitve SharePoint ali OneDrive

Ko poskušate uporabiti SharePoint ali OneDrive za enega od naslednjih scenarijev, lahko uporabniki prejmejo sporočilo **za vzdrževanje samo za branje** . 

-   Načrtovana ali aktivna vzdrževalna dejavnost.  Preverite jih tako, da se pomaknete na [center za sporočila](https://portal.office.com/adminportal/home#/messagecenter).
-   Zelo prednostna, aktivna storitev incident, ki se lahko pojavijo. Preverite za morebitne Advisories/incidentov, ki jih navigacija do [storitve Health](https://portal.office.com/adminportal/home#/servicehealth).
-   Manjše okrevanje Auto-Healing scenarij, ki bi se lahko dogajalo zaradi kakršnih koli nepričakovanih dogodkov na strežnikih, ki bi lahko trajala manj kot 30 min ali tako. 
    
    Ni sporočila center ali Service Health delovnih mest za te manjše izterjave, vendar bi morali biti nazaj na normalno zelo kmalu.

Ob zelo redkih priložnostih smo opazili, da je eden od treh zgoraj naštetih scenarijev je bil vzrok, in storitev je bila obnovljena, vendar uporabniki brskalnika predpomnilnik ni bil očiščen.

Pred navigacijo do spletnega mesta poskusite počistiti predpomnilnik brskalnika.

1. V brskalniku Microsoft Edge izberite **Nastavitve**, nato pa izberite **zasebnost in varnost**.
2. Pod možnostjo **Izbriši brskanje**izberite izberite **, kaj želite počistiti**.
3. Izberite **piškotki in shranjeni podatki spletnega mesta**ter izberite **Počisti**.

>[!Note] 
> Ti koraki se lahko razlikujejo pri uporabi drugih brskalnikov, kot sta Mozilla Firefox ali Google Chrome.

>[!Note] 
> Druga možnost bi bila, da odprete SharePointovo spletno mesto ali OneDrive v novem oknu InPrivate.