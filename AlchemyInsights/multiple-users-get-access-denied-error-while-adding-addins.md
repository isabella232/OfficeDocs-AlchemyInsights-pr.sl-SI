---
title: Več uporabnikov dobi napako »Dostop zavrnjeno« med dodajanjem dodatkov v programu Outlook
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
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424175"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="90c95-102">Več uporabnikov dobi napako »Dostop zavrnjeno« med dodajanjem dodatkov v programu Outlook</span><span class="sxs-lookup"><span data-stu-id="90c95-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="90c95-103">Določite lahko, kateri skrbniki v organizaciji imajo dovoljenja za namestitev in upravljanje dodatkov za Outlook.</span><span class="sxs-lookup"><span data-stu-id="90c95-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="90c95-104">Določite lahko tudi, kateri uporabniki v vaši organizaciji imajo dovoljenje za namestitev in upravljanje dodatkov za lastno uporabo.</span><span class="sxs-lookup"><span data-stu-id="90c95-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="90c95-105">Če želite podrobnosti, [glejte Določanje skrbnikov in uporabnikov, ki lahko namestijo in upravljajo dodatke za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="90c95-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="90c95-106">Če želite preveriti, ali ste uporabniku uspešno dodelili dovoljenja, <Role Name> zamenjajte z imenom vloge, ki jo želite preveriti, in zaženite ta ukaz v lupini PowerShell za Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="90c95-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="90c95-107">Get-ManagementRoleAssignment -Vloga " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="90c95-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="90c95-108">V tem primeru je prikazano, kako preverite, komu ste dodelili dovoljenja za namestitev dodatkov iz Trgovine Office za organizacijo.</span><span class="sxs-lookup"><span data-stu-id="90c95-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="90c95-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="90c95-109">PowerShell</span></span>

<span data-ttu-id="90c95-110">-Vloga "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="90c95-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="90c95-111">V rezultatih, Get-ManagementRoleAssignment, preglejte vnose v stolpcu Učinkovite uporabnike.</span><span class="sxs-lookup"><span data-stu-id="90c95-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="90c95-112">Za podrobne informacije o sintaksi in parametrih [glejte Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="90c95-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 