---
title: En uporabnik ne vidi dodatkov v programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198220"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="e892c-102">En uporabnik ne vidi dodatkov v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="e892c-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="e892c-103">Uporabnik je morda del vloge, ki nima pravilnega parametra AppsForOfficeEnabled.</span><span class="sxs-lookup"><span data-stu-id="e892c-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="e892c-104">Zaženite ta ukaz» cmdlet «, če želite izvedeti, ali je pravilna vloga povezana z uporabnikom:</span><span class="sxs-lookup"><span data-stu-id="e892c-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="e892c-105">Get-Managementroleodstop-RoleAssignee user@domain.com-delegiranje $false | Format-table-Auto vlogo, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="e892c-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="e892c-106">Če želite več informacij, glejte [določanje skrbnikov in uporabnikov, ki lahko namestijo in upravljajo dodatke za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="e892c-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
