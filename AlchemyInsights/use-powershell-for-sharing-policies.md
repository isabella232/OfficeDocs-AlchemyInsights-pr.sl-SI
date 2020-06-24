---
title: Uporaba pravilnikov PowerShell za skupno rabo in odnosov organizacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862156"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="40d05-102">Uporaba pravilnikov PowerShell za skupno rabo in odnosov organizacije</span><span class="sxs-lookup"><span data-stu-id="40d05-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="40d05-103">Za odnose organizacije preglejte podrobne podatke o skladnji in parametrih za: [pridobite-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [set-Organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) in [Odstrani-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="40d05-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="40d05-104">Če želite ustvariti pravilnik za skupno rabo, uporabite [novo pravilnik](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="40d05-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="40d05-105">Če želite [uporabiti pravilnik o skupni rabi za nabiralnik ali uporabnika](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) , morate uporabiti kombinacijo [set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) in [zaslužiti-poštni nabiralnik](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) z novo ustvarjeno politiko.</span><span class="sxs-lookup"><span data-stu-id="40d05-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="40d05-106">V [ublažiti, onesposobiti ali premestitev a črepina zvitost](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) vi potreba rabiti [število enakih oseb-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) ter [premestitev-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="40d05-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="40d05-107">**Za popolno razumevanje te teme preberite:**</span><span class="sxs-lookup"><span data-stu-id="40d05-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="40d05-108">Skupna raba v Exchange Online</span><span class="sxs-lookup"><span data-stu-id="40d05-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)