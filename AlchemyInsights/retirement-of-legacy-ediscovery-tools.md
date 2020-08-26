---
title: Upokojitev podedovanih E-odkrivanje orodij
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902636"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="c68b6-102">Upokojitev podedovanih E-odkrivanje orodij</span><span class="sxs-lookup"><span data-stu-id="c68b6-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="c68b6-103">Kot rezultat nove in izboljšane funkcije E-odkrivanje v središču za skladnost s predpisi Microsoft 365 se bodo v prihodnjih mesecih umaknila naslednja podedovana E-odkrivanje orodja in ukazov:</span><span class="sxs-lookup"><span data-stu-id="c68b6-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="c68b6-104">[Na mestu e-odkrivanje](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) in [na](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) mestu uporabe v skrbniškem središču za Exchange.</span><span class="sxs-lookup"><span data-stu-id="c68b6-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="c68b6-105">Ukazi» cmdlet «za Exchange Online, ki podpirajo na mestu E-odkrivanje in na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="c68b6-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="c68b6-106">(Ti ukazi» cmdlet «so skupaj opredeljeni kot \*-MailboxSearch ukazi» cmdlet «.) To vključuje te ukaze» cmdlet «:</span><span class="sxs-lookup"><span data-stu-id="c68b6-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="c68b6-107">Novo-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c68b6-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="c68b6-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c68b6-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="c68b6-109">Zaustavitev-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c68b6-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="c68b6-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="c68b6-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="c68b6-111">Ukaz» cmdlet « [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v storitvi Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c68b6-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="c68b6-112">Te operacije v API-jih storitve Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="c68b6-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="c68b6-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="c68b6-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="c68b6-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c68b6-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="c68b6-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="c68b6-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="c68b6-116">Napredno E-odkrivanje v 1.0</span><span class="sxs-lookup"><span data-stu-id="c68b6-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="c68b6-117">**Časovnica za upokojitev**:</span><span class="sxs-lookup"><span data-stu-id="c68b6-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="c68b6-118">**1. julij 2020** Ne morete več ustvarjati novih iskanj in jih prihraniti, lahko pa zaganjate, urejate in brišete obstoječa iskanja na lastno odgovornost.</span><span class="sxs-lookup"><span data-stu-id="c68b6-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="c68b6-119">Microsoftova podpora ni več podprta na mestu E-odkrivanje, & ima v programu EAC.</span><span class="sxs-lookup"><span data-stu-id="c68b6-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="c68b6-120">**1. oktober 2020** Na mestu E-odkrivanje & funkcija ima funkcionalnost v programu EAC, ki bo v načinu samo za branje, zato lahko odstranite le obstoječa iskanja in zadržanje.</span><span class="sxs-lookup"><span data-stu-id="c68b6-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="c68b6-121">Če **želite več informacij, glejte**:</span><span class="sxs-lookup"><span data-stu-id="c68b6-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="c68b6-122">Selitev podedovanih E-odkrivanje iskanj in zadržanje v središču za skladnost s predpisi Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c68b6-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="c68b6-123">Upokojitev podedovanih E-odkrivanje orodij</span><span class="sxs-lookup"><span data-stu-id="c68b6-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="c68b6-124">Pogosta vprašanja o E-odkrivanje na mestu uporabe in na mestu uporabe</span><span class="sxs-lookup"><span data-stu-id="c68b6-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



