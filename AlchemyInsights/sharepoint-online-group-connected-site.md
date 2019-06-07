---
title: Dodaj skupino na SharePointovo mesto
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758746"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Ustvarite skupino povezanih stran v SharePoint Online

Obstaja nekaj skupnih problemov ko ustvarjanje ali znova ustvarite skupino povezanih strani.

 Če boste izbrisali skupino in njene povezane strani in želijo ustvariti drugo mesto z enakim URL-jem, potrebovali boste trajno odstranili prejšnjega mesta.

Travnato gričevje [ukazno lupino za upravljanje SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Več informacij na uvod v powershell, glejte [Uvod v SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Odstraniti mesto od izbrisati strani, ki uporabljajo [Odstrani-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.

Če ustvarjate skupine povezanih strani in prejmete opozorilo že obstaja še skupina z enako alias, preverite obstoječe skupine iz [Office 365 od Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Odpravili, izbrisati obstoječo skupino, če to ni več potrebna ali ustvarite strani z različnimi alias dodeljen.

Obstajajo različne načine za ustvarjanje in uporabo sodobnih skupine s SharePointom.

Priključite obstoječih mestih Office 365 skupini. Za več informacij, glejte [povezovanje skupino Office 365 uporabljajo SharePoint uporabnik ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Tvoriti Office 365 skupina povezanih strani, boste morali ustvariti mesto ekipa. Za več informacij, glejte [ustvarjanje mesta skupine SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

