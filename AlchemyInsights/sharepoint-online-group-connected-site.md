---
title: Dodajanje skupine na SharePoint mestu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318140"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Pogoste težave pri ustvarjanju povezanega spletnega mesta skupine v SharePoint

1. Če ste izbrisali skupino in povezano spletno mesto ter želite ustvariti še eno mesto z istim URL-jem, boste morali trajno odstraniti prejšnje mesto.

   - Prenos [lupine za upravljanje SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Če želite več informacij o tem, kako začeti uporabljati Powershell, [glejte Uvod v lupino za SharePoint Online.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Odstranite mesto z izbrisanih mest z ukazom »cmdlet« [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Če želite trajno izbrisati mesta skupine, potrebujete Powershell.

1. Če ustvarjate spletno mesto, povezano s skupino, in prejmete **opozorilo:** Druga skupina z istim vzdevki že obstaja, preverite obstoječe skupine v [Skrbniško središče za Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Če želite odpraviti težavo, izbrišite obstoječo skupino, če je ne potrebujete več, ali pa ustvarite mesto z drugim vzdevki.

1. Obstaja več načinov za ustvarjanje in uporabo sodobnih skupin v SharePoint.

   - Obstoječa mesta lahko povežete s skupino Microsoft 365 mest. Če želite več informacij, [Povezovalnik skupino Microsoft 365 prek SharePoint vmesnika.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Če želite Microsoft 365 spletno mesto, povezano s skupino, morate ustvariti spletno [mesto skupine.](https://admin.microsoft.com/sharepoint)
