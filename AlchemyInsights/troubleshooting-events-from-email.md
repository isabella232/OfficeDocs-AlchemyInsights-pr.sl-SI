---
title: Odpravljanje težav z e-pošto
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658750"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="6bc5e-102">Odpravljanje težav z e-pošto</span><span class="sxs-lookup"><span data-stu-id="6bc5e-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="6bc5e-103">Preverite, ali je funkcija omogočena za nabiralnik: **Get-EventsFromEmailConfiguration- <mailbox> Identity**</span><span class="sxs-lookup"><span data-stu-id="6bc5e-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="6bc5e-104">Nato si oglejte dnevniki» dogodki iz e-pošte « **Izvozi – MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="6bc5e-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="6bc5e-105">V dnevnikih» dogodki iz e-pošte «poiščite InternetMessageId, ki se ujema z elementom v nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="6bc5e-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="6bc5e-106">TrustScore določi, ali je element dodan ali ne.</span><span class="sxs-lookup"><span data-stu-id="6bc5e-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="6bc5e-107">Dogodki bodo dodani le, če je TrustScore = "zaupanja vreden".</span><span class="sxs-lookup"><span data-stu-id="6bc5e-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="6bc5e-108">TrustScore je določen z lastnostmi SPF, DKIM ali dMarc, ki so v glavi sporočila.</span><span class="sxs-lookup"><span data-stu-id="6bc5e-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="6bc5e-109">Če si želite ogledati te lastnosti:</span><span class="sxs-lookup"><span data-stu-id="6bc5e-109">To view these properties:</span></span>

<span data-ttu-id="6bc5e-110">**Namizni Outlook**</span><span class="sxs-lookup"><span data-stu-id="6bc5e-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="6bc5e-111">Odpiranje elementa</span><span class="sxs-lookup"><span data-stu-id="6bc5e-111">Open the item</span></span>
- <span data-ttu-id="6bc5e-112">Lastnosti datoteke >-> internetne glave</span><span class="sxs-lookup"><span data-stu-id="6bc5e-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="6bc5e-113">ali</span><span class="sxs-lookup"><span data-stu-id="6bc5e-113">or</span></span>

<span data-ttu-id="6bc5e-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="6bc5e-114">**MFCMapi**</span></span>

- <span data-ttu-id="6bc5e-115">Pomikanje do elementa v mapi» Prejeto «</span><span class="sxs-lookup"><span data-stu-id="6bc5e-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="6bc5e-116">Poiščite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="6bc5e-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="6bc5e-117">Te lastnosti so določene in zabeležene med prevozom in usmerjanjem.</span><span class="sxs-lookup"><span data-stu-id="6bc5e-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="6bc5e-118">Če želite dodatno odpraviti težave, boste morda morali nadaljevati s podporo za prenos informacij o napakah v SPF, DKIM in. or DMARC.</span><span class="sxs-lookup"><span data-stu-id="6bc5e-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>