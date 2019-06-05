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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719497"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Ustvarite skupino povezanih stran v SharePoint Online

<p><strong>Obstaja nekaj skupnih problemov ko ustvarjanje ali znova ustvarite skupino povezanih strani.&nbsp;</strong></p>  <p>1.Če boste izbrisali skupino in njene povezane strani in želijo ustvariti drugo mesto z enakim URL-jem, potrebovali boste trajno odstranili prejšnjega mesta.</p>  <ul>  <li>Travnato gričevje <a title="ukazno lupino za upravljanje SPO" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO Management Shell</a> - za več informacij o uvod v powershell, glejte <a title="uvod v SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Uvod v SharePoint Online Management Shell</a>. <br /><br /></li>  <li>Odstranite izbrisane strani z uporabo strani se <a title="premestitev-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Odstrani-SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Če ustvarjate skupine povezanih strani in prejmete opozorilo <strong>'druga skupina istem alias že obstaja'</strong>, preverite obstoječe skupine v <a title="Office 365 od Admin Center" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 od Admin Center</a>. Odpravili, izbrisati obstoječo skupino, če to ni več potrebna ali ustvarite strani z različnimi alias dodeljen.&nbsp;</p>  <p><strong>Obstajajo različne načine za ustvarjanje in uporabo sodobnih skupine s SharePointom.&nbsp;</strong></p>  <ol>  <li>Priključite obstoječih mestih Office 365 skupini. Več informacij, si oglejte <a title="povezavo z Office 365 skupino SharePoint uporabnik ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Povezavo z Office 365 skupino SharePoint uporabnik ineterface</a>.</li>  <li>Tvoriti Office 365 skupina povezanih strani, boste morali ustvariti mesto ekipa. Več informacij, si oglejte <a title="ustvariti mesto ekipa v SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Ustvarite mesto ekipe v SharePoint.</a></li>  </ol>

