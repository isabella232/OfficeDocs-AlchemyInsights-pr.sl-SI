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
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="2a406-102">Ustvarite skupino povezanih stran v SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2a406-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="2a406-103">Obstaja nekaj skupnih problemov ko ustvarjanje ali znova ustvarite skupino povezanih strani.</span><span class="sxs-lookup"><span data-stu-id="2a406-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="2a406-104">Če boste izbrisali skupino in njene povezane strani in želijo ustvariti drugo mesto z enakim URL-jem, potrebovali boste trajno odstranili prejšnjega mesta.</span><span class="sxs-lookup"><span data-stu-id="2a406-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="2a406-105">Travnato gričevje [ukazno lupino za upravljanje SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="2a406-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="2a406-106">Več informacij na uvod v powershell, glejte [Uvod v SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="2a406-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="2a406-107">Odstraniti mesto od izbrisati strani, ki uporabljajo [Odstrani-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="2a406-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="2a406-108">Če ustvarjate skupine povezanih strani in prejmete opozorilo že obstaja še skupina z enako alias, preverite obstoječe skupine iz [Office 365 od Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="2a406-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="2a406-109">Odpravili, izbrisati obstoječo skupino, če to ni več potrebna ali ustvarite strani z različnimi alias dodeljen.</span><span class="sxs-lookup"><span data-stu-id="2a406-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="2a406-110">Obstajajo različne načine za ustvarjanje in uporabo sodobnih skupine s SharePointom.</span><span class="sxs-lookup"><span data-stu-id="2a406-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="2a406-111">Priključite obstoječih mestih Office 365 skupini.</span><span class="sxs-lookup"><span data-stu-id="2a406-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="2a406-112">Za več informacij, glejte [povezovanje skupino Office 365 uporabljajo SharePoint uporabnik ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="2a406-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="2a406-113">Tvoriti Office 365 skupina povezanih strani, boste morali ustvariti mesto ekipa.</span><span class="sxs-lookup"><span data-stu-id="2a406-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="2a406-114">Za več informacij, glejte [ustvarjanje mesta skupine SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="2a406-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

