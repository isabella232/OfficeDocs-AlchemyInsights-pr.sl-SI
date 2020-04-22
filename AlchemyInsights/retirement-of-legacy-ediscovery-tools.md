---
title: Upokojitev Legacy orodja e-odkrivanja
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650584"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="98811-102">Upokojitev Legacy orodja e-odkrivanja</span><span class="sxs-lookup"><span data-stu-id="98811-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="98811-103">Zaradi nove in izboljšane funkcionalnosti e-odkrivanja v Microsoftovem 365 centru za skladnost bodo v naslednjih mesecih upokojeni naslednji podedovani orodji e-discovery in Commandlets:</span><span class="sxs-lookup"><span data-stu-id="98811-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="98811-104">In [-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) in [v mestu ima](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v skrbniškem središču Exchange.</span><span class="sxs-lookup"><span data-stu-id="98811-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="98811-105">Cmdlets za Exchange Online PowerShell, ki podpirajo e-odkrivanje in-Place v mestu.</span><span class="sxs-lookup"><span data-stu-id="98811-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="98811-106">(Ti ukazi» cmdlet «so skupno označeni kot» cmdlet «-MailboxSearch.) To vključuje naslednje ukaze» cmdlet «:</span><span class="sxs-lookup"><span data-stu-id="98811-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="98811-107">Novo-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="98811-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="98811-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="98811-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="98811-109">Zaustavitev-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="98811-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="98811-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="98811-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="98811-111">Ukaz» cmdlet «za [Iskanje-nabiralnik](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v PowerShell Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="98811-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="98811-112">Naslednje operacije v API-ju storitve Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="98811-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="98811-113">Getsearchablenabiralniki</span><span class="sxs-lookup"><span data-stu-id="98811-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="98811-114">Setholdonnabiralniki</span><span class="sxs-lookup"><span data-stu-id="98811-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="98811-115">Getholdonnabiralniki</span><span class="sxs-lookup"><span data-stu-id="98811-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="98811-116">Napredno eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="98811-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="98811-117">**Časovna premica za upokojitev**:</span><span class="sxs-lookup"><span data-stu-id="98811-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="98811-118">1. april 2020: ne boste mogli ustvariti novih iskanj in zadržanj, vendar lahko še vedno zaženete, urejate in izbrišete obstoječa iskanja na lastno odgovornost.</span><span class="sxs-lookup"><span data-stu-id="98811-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="98811-119">Microsoftova podpora ne bo več podpirala in-Place eDiscovery & zadržki v EAC.</span><span class="sxs-lookup"><span data-stu-id="98811-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="98811-120">1. julij 2020: funkcija eDiscovery & na mestu delovanja v EAC bo postavljena v način samo za branje.</span><span class="sxs-lookup"><span data-stu-id="98811-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="98811-121">To pomeni, da boste lahko odstranili obstoječa iskanja in zadržki.</span><span class="sxs-lookup"><span data-stu-id="98811-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="98811-122">**Za več informacij glejte**:</span><span class="sxs-lookup"><span data-stu-id="98811-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="98811-123">Selitev podedovanih iskanj e-odkrivanja in skladišč v središče za skladnost z Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="98811-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="98811-124">Upokojitev starejših orodij e-odkrivanja</span><span class="sxs-lookup"><span data-stu-id="98811-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="98811-125">Pogosta vprašanja o eDiscovery v mestu in kraju</span><span class="sxs-lookup"><span data-stu-id="98811-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



