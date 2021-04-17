---
title: Odpravljanje težav z dogodki iz e-pošte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834855"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="cba80-102">Odpravljanje težav z dogodki iz e-pošte</span><span class="sxs-lookup"><span data-stu-id="cba80-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="cba80-103">Preverite, ali je funkcija omogočena za nabiralnik: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="cba80-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="cba80-104">Nato si oglejte dnevnike »Dogodki iz **e-pošte« Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="cba80-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="cba80-105">V dnevnikih »Dogodki iz e-pošte« poiščite IDza InternetMessageId, ki se ujema z elementom v nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="cba80-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="cba80-106">TrustScore določi, ali je element dodan ali ne.</span><span class="sxs-lookup"><span data-stu-id="cba80-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="cba80-107">Dogodki bodo dodani le, če je TrustScore = »Zaupanja vreden«.</span><span class="sxs-lookup"><span data-stu-id="cba80-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="cba80-108">TrustScore določa lastnosti SPF, Dkim ali Dmarc, ki so v glavi sporočila.</span><span class="sxs-lookup"><span data-stu-id="cba80-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="cba80-109">Če si želite ogledati te lastnosti:</span><span class="sxs-lookup"><span data-stu-id="cba80-109">To view these properties:</span></span>

<span data-ttu-id="cba80-110">**Namizna različica Outlooka**</span><span class="sxs-lookup"><span data-stu-id="cba80-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="cba80-111">Odpiranje elementa</span><span class="sxs-lookup"><span data-stu-id="cba80-111">Open the item</span></span>
- <span data-ttu-id="cba80-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="cba80-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="cba80-113">ali</span><span class="sxs-lookup"><span data-stu-id="cba80-113">or</span></span>

<span data-ttu-id="cba80-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="cba80-114">**MFCMapi**</span></span>

- <span data-ttu-id="cba80-115">Krmarjenje do elementa v mapi »Prejeto«</span><span class="sxs-lookup"><span data-stu-id="cba80-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="cba80-116">Poiščite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="cba80-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="cba80-117">Te lastnosti so določene in zapisane med transportom in usmerjanjem.</span><span class="sxs-lookup"><span data-stu-id="cba80-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="cba80-118">Za dodatno odpravljanje težav boste morda morali upoštevati podporo za prenos v zvezi z napakami v SPF, DKIM in.or DMARC.</span><span class="sxs-lookup"><span data-stu-id="cba80-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>