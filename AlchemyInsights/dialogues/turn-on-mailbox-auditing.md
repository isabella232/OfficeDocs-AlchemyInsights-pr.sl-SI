---
title: Vklop nadzora nabiralnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429743"
---
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="fbd56-102">Vklop nadzora nabiralnika</span><span class="sxs-lookup"><span data-stu-id="fbd56-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="fbd56-103">Če želite vklopiti nadzor nabiralnika za enega uporabnika ali celotno organizacijo, zaženite te ukaze» cmdlet «iz oddaljenega PowerShella:</span><span class="sxs-lookup"><span data-stu-id="fbd56-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="fbd56-104">**En uporabnik**: Set-Mailbox-Identity "Jane Dow"-AuditEnabled $True</span><span class="sxs-lookup"><span data-stu-id="fbd56-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="fbd56-105">**Organizacija**: Get-Mailbox-ResultSize Unlimited-filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="fbd56-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="fbd56-106">Če želite izvedeti več, glejte [upravljanje nadzora nabiralnika](https://go.microsoft.com/fwlink/?linkid=2103668).</span><span class="sxs-lookup"><span data-stu-id="fbd56-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>