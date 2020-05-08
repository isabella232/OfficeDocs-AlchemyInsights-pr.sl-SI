---
title: Dodajanje skupine na SharePointovo mesto
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: b54457427ffa563b6a6323d85e1c8800191eca11
ms.sourcegitcommit: d1aad215f8aa636ba89c93a13a0c9d90e997f752
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/06/2020
ms.locfileid: "44064409"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Težave pri ustvarjanju skupine, povezane z mestom v SharePointu

1. Nekatera pogosta vprašanja, ki so se pojavile pri ustvarjanju ali vnovični vzpostavitvi povezanega spletnega mesta skupine.
Če ste izbrisali skupino in njeno povezano spletno mesto in želite ustvariti drugo spletno mesto z istim URL-jem, boste morali trajno odstraniti prejšnje mesto.

   - Travnato gričevje [spo uprava skorja](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Če želite več informacij o tem, kako začeti z lupino PowerShell, glejte [Uvod v SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Odstranite stran iz izbrisanih mest z ukazom» cmdlet « [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. PowerShell je treba trajno izbrisati skupine mest.

1. Če ustvarjate skupinsko povezano mesto in prejmete opozorilo: **druga skupina z istim vzdevkom že obstaja**, preverite obstoječe skupine iz [skrbniškega središča Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Če želite odpraviti težavo, izbrišite obstoječo skupino, če je ni več potrebno ali ustvarite mesto z drugim dodeljenim vzdevkom.

1. Obstajajo različni načini za ustvarjanje in uporabo sodobnih skupin s SharePointom.

   - Obstoječa mesta lahko povežete s skupino Microsoft 365. Če želite več informacij, glejte [povezovanje skupine Microsoft 365 s SharePointovim uporabniškim vmesnikom](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Če želite ustvariti povezano spletno mesto skupine Microsoft 365, morate ustvariti [spletno mesto skupine](https://admin.microsoft.com/sharepoint).
