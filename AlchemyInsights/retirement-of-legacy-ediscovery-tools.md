---
title: Upokojitev podedovanih orodij za e-odkrivanje
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798565"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="12682-102">Upokojitev podedovanih orodij za e-odkrivanje</span><span class="sxs-lookup"><span data-stu-id="12682-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="12682-103">Zaradi nove in izboljšane funkcije e-odkrivanja v središču za skladnost s predpisi storitve Microsoft 365 bodo v prihodnjih mesecih ukinjena ta podedovana orodja za e-odkrivanje in ukazni ukazi:</span><span class="sxs-lookup"><span data-stu-id="12682-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="12682-104">[E-odkrivanje na mestu](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [in zadržanja na mestu v](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) skrbniškem središču za Exchange.</span><span class="sxs-lookup"><span data-stu-id="12682-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="12682-105">Ukazi »cmdlet« lupine PowerShell za Exchange Online, In-Place e-odkrivanje in In-Place zadržanja.</span><span class="sxs-lookup"><span data-stu-id="12682-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="12682-106">(Te ukaze »cmdlet« je mogoče skupaj določiti kot ukaze »cmdlet« \*-MailboxSearch.) To vključuje te ukaze »cmdlet«:</span><span class="sxs-lookup"><span data-stu-id="12682-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="12682-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="12682-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="12682-108">Iskanje po začetnem nabiralniku</span><span class="sxs-lookup"><span data-stu-id="12682-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="12682-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="12682-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="12682-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="12682-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="12682-111">Ukaz [»cmdlet« za iskanje](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v nabiralniku v lupini PowerShell za Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="12682-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="12682-112">Te operacije v VMESNIKU API za Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="12682-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="12682-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="12682-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="12682-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="12682-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="12682-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="12682-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="12682-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="12682-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="12682-117">**Časovnica za upokojitev:**</span><span class="sxs-lookup"><span data-stu-id="12682-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="12682-118">**1. julij 2020** Ne morete več ustvarjati novih iskan in zadržanj, lahko pa izvajate, urejate in brišete obstoječa iskanja na lastno odgovornost.</span><span class="sxs-lookup"><span data-stu-id="12682-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="12682-119">Microsoftova podpora ne podpira več In-Place zadržanj e-& v EAC.</span><span class="sxs-lookup"><span data-stu-id="12682-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="12682-120">**1. oktober 2020** In-Place funkcijo e-odkrivanja & Zadržanja bodo v EAC postavljena v način samo za branje, tako da lahko odstranite le obstoječa iskanja in zadržanja.</span><span class="sxs-lookup"><span data-stu-id="12682-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="12682-121">**Če želite več informacij, glejte:**</span><span class="sxs-lookup"><span data-stu-id="12682-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="12682-122">Selitev podedovanih iskancev e-odkrivanja in zadržanja v središče za skladnost s predpisi storitve Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="12682-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="12682-123">Umik podedovanih orodij za e-odkrivanje</span><span class="sxs-lookup"><span data-stu-id="12682-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="12682-124">Pogosta vprašanja o In-Place e-odkrivanju in In-Place zadržanjih</span><span class="sxs-lookup"><span data-stu-id="12682-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



