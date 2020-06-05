---
title: Odpravljanje težav pri dogodkih iz e-pošte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569403"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="faa79-102">Odpravljanje težav pri dogodkih iz e-pošte</span><span class="sxs-lookup"><span data-stu-id="faa79-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="faa79-103">Preverite, ali je funkcija omogočena za nabiralnik: \*\*zaslužiti-EventsFromEmailConfiguration-identiteta <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="faa79-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="faa79-104">Potem poglej "dogodki iz e-pošte" dnevniki **Export-Mailboxdiagnosticdnevniki <mailbox> -Component timeprofile**</span><span class="sxs-lookup"><span data-stu-id="faa79-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="faa79-105">V dnevnikih» dogodki iz e-pošte «poiščite InternetMessageId, ki se ujema z elementom v nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="faa79-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="faa79-106">Vrednost TrustScore določa, ali je artikel dodan ali ne.</span><span class="sxs-lookup"><span data-stu-id="faa79-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="faa79-107">Dogodki bodo dodani le, če je TrustScore = "zaupanja vreden".</span><span class="sxs-lookup"><span data-stu-id="faa79-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="faa79-108">TrustScore določa lastnosti SPF, DKIM ali dMarc, ki so v glavi sporočila.</span><span class="sxs-lookup"><span data-stu-id="faa79-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="faa79-109">Če si želite ogledati te lastnosti:</span><span class="sxs-lookup"><span data-stu-id="faa79-109">To view these properties:</span></span>

<span data-ttu-id="faa79-110">**Namizni obeti**</span><span class="sxs-lookup"><span data-stu-id="faa79-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="faa79-111">Odpiranje elementa</span><span class="sxs-lookup"><span data-stu-id="faa79-111">Open the item</span></span>
- <span data-ttu-id="faa79-112">Datoteke-lastnosti >-> internetne glave</span><span class="sxs-lookup"><span data-stu-id="faa79-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="faa79-113">Ali</span><span class="sxs-lookup"><span data-stu-id="faa79-113">or</span></span>

<span data-ttu-id="faa79-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="faa79-114">**MFCMapi**</span></span>

- <span data-ttu-id="faa79-115">Pomikanje do elementa v mapi» Prejeto «</span><span class="sxs-lookup"><span data-stu-id="faa79-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="faa79-116">Poiščite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="faa79-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="faa79-117">Te lastnosti se določijo in zabeležijo med transportom in usmerjanjem.</span><span class="sxs-lookup"><span data-stu-id="faa79-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="faa79-118">Za nadaljnje odpravljanje težav boste morda morali spremljati prometno podporo o napakah v SPF, DKIM in. ali DMARC.</span><span class="sxs-lookup"><span data-stu-id="faa79-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>