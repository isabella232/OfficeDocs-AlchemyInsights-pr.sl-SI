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
ms.openlocfilehash: 6aea12d44a44a3e11eaf3fb1bd47ff3e9dbfd9e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507863"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Vprašanja pri ustvarjanju ali skupina povezanih mest v SharePoint Online

Obstaja nekaj skupnih problemov ko ustvarjanje ali znova ustvarite skupino povezanih strani.

 Če boste izbrisali skupino in njene povezane strani in želijo ustvariti drugo mesto z enakim URL-jem, potrebovali boste trajno odstranili prejšnjega mesta.

Travnato gričevje [ukazno lupino za upravljanje SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Več informacij na uvod v powershell, glejte [Uvod v SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

Odstraniti mesto od izbrisati strani, ki uporabljajo [Odstrani-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.

Če ustvarjate skupine povezanih strani in prejmete opozorilo že obstaja še skupina z enako alias, preverite obstoječe skupine iz [Office 365 od Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Odpravili, izbrisati obstoječo skupino, če to ni več potrebna ali ustvarite strani z različnimi alias dodeljen.

Obstajajo različne načine za ustvarjanje in uporabo sodobnih skupine s SharePointom.

Priključite obstoječih mestih Office 365 skupini. Za več informacij, glejte [povezovanje skupino Office 365 uporabljajo SharePoint uporabnik ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).

Tvoriti Office 365 skupina povezanih strani, boste morali ustvariti mesto ekipa. Za več informacij, glejte [ustvarjanje mesta skupine SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

