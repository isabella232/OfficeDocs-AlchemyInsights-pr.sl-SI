---
title: 'Vloge RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583953"
---
# <a name="rbac-rules"></a><span data-ttu-id="7eb52-102">Pravila RBAC</span><span class="sxs-lookup"><span data-stu-id="7eb52-102">RBAC rules</span></span>

<span data-ttu-id="7eb52-103">Če se prikaže napaka» dovoljenje «:</span><span class="sxs-lookup"><span data-stu-id="7eb52-103">If you get the permission error:</span></span> 

- <span data-ttu-id="7eb52-104">**Odjemalec z ID-jem predmeta nima dovoljenja za izvajanje dejanj nad obsegom (koda: AuthorizationFailed)**: ko poskušate ustvariti vir, preverite, ali ste trenutno vpisani z uporabnikom, ki je dodeljen vlogi, ki ima dovoljenje za pisanje za vir v izbranem obsegu.</span><span class="sxs-lookup"><span data-stu-id="7eb52-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="7eb52-105">Če želite na primer upravljati virtualne stroje v skupini virov, morate imeti vlogo [navideznega stroja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) v skupini virov (ali nadrejenem obsegu).</span><span class="sxs-lookup"><span data-stu-id="7eb52-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="7eb52-106">Če želite seznam dovoljenj za vsako vgrajeno vlogo, glejte [vgrajene vloge za vire Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="7eb52-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="7eb52-107">Nimate **dovoljenja za ustvarjanje zahteve za podporo**: ko poskušate ustvariti ali posodobiti vstopnico za podporo, se prepričajte, da ste trenutno vpisani z uporabnikom, ki je dodeljen vlogi, ki ima Microsoftovo dovoljenje za podporo/supportTickets/pisanje, kot je na primer [Podpora za zahtevo](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="7eb52-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="7eb52-108">**Ne morete ustvariti več dodelitev vlog (koda: RoleAssignmentLimitExceeded)**: ko poskušate dodeliti vlogo, poskusite zmanjšati število dodelitev vlog tako, da dodelite vloge skupinam.</span><span class="sxs-lookup"><span data-stu-id="7eb52-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="7eb52-109">Azure podpira do **2000** dodelitev vlog na naročnino.</span><span class="sxs-lookup"><span data-stu-id="7eb52-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="7eb52-110">Če želite več informacij o vlogah Azure RBAC, glejte vloge v storitvi [AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="7eb52-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
