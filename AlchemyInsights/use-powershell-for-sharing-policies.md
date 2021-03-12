---
title: Uporaba PowerShell za skupno rabo pravilnikov in odnosov organizacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709482"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="5bbb1-102">Uporaba PowerShell za skupno rabo pravilnikov in odnosov organizacije</span><span class="sxs-lookup"><span data-stu-id="5bbb1-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="5bbb1-103">Za odnose organizacije si oglejte podrobno sintakso in informacije o parametrih za: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="5bbb1-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="5bbb1-104">Če želite ustvariti pravilnik o skupni rabi, [»New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="5bbb1-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="5bbb1-105">Če želite uporabiti[pravilnik za skupno rabo za nabiralnik ali uporabnika](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  morate uporabiti kombinacijo  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) in [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) z novo ustvarjenim pravilnikom.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="5bbb1-106">Če  [spremeniti, onemogočiti ali odstraniti pravilnik o skupni rabi](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  morate uporabiti  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) in [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="5bbb1-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="5bbb1-107">**Za popolno razumevanje te teme preberite:**</span><span class="sxs-lookup"><span data-stu-id="5bbb1-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="5bbb1-108">Skupna raba v programu Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5bbb1-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)