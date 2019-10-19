---
title: Dodajanje skupine na SharePointovo mesto
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750536"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Težave pri ustvarjanju ali združevanje povezanih mest v SharePoint online

Pri ustvarjanju ali ponovnem ustvarjanju skupine, ki je povezana s skupino, je prišlo do nekaj pogostih težav.

 Če ste izbrisali skupino in njeno povezano spletno mesto in želite ustvariti drugo spletno mesto z istim URL-jem, boste morali trajno odstraniti prejšnje mesto.

Travnato gričevje [spo uprava skorja](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Če želite več informacij o tem, kako začeti z lupino PowerShell, glejte [Uvod v SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Odstranite stran iz izbrisanih mest z ukazom» cmdlet « [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell.

Če ustvarjate skupinsko povezano spletno mesto in prejmete opozorilo druga skupina z istim vzdevkom že obstaja, preverite obstoječe skupine iz [officea 365 iz skrbniškega središča](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Če želite odpraviti težavo, izbrišite obstoječo skupino, če je ni več potrebno ali ustvarite mesto z drugim dodeljenim vzdevkom.

Obstajajo različni načini za ustvarjanje in uporabo sodobnih skupin s SharePointom.

Obstoječa mesta lahko povežete s skupino Office 365. Če želite več informacij, glejte [povezovanje skupine Office 365 s SharePointovim uporabniškim obrazom](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Če želite ustvariti povezano spletno mesto skupine Office 365, morate ustvariti spletno mesto skupine. Če želite več informacij, glejte [ustvarjanje mesta ekipe v SharePointu](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

