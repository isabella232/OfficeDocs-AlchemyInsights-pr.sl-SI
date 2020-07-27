---
title: En uporabnik dobi napako pri dostopu zavrnjene napake pri dodajanju dodatkov v programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 1f4672e306a282b3e1d20c75f4e361c02cdddaed
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424186"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="c2917-102">En uporabnik dobi napako pri dostopu zavrnjene napake pri dodajanju dodatkov v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="c2917-102">One user gets Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="c2917-103">User PowerShell Če želite poiskati dovoljenja:</span><span class="sxs-lookup"><span data-stu-id="c2917-103">User PowerShell To find permissions:</span></span>

<span data-ttu-id="c2917-104">Get-ManagementRoleAssignment -RoleAssignee [user@domain.com-Prenos](mailto:user@domain.com "mailto:user@domain.com") $false | Oblika-tabela -Auto vloga,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="c2917-104">Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>