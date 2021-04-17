---
title: Ali potrebujete pomoč za omejitve pošiljanja e-pošte?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836295"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="6679f-102">Ali potrebujete pomoč za omejitve pošiljanja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="6679f-102">Need help with email sending limits?</span></span>

<span data-ttu-id="6679f-103">Spodaj so navedene **privzete omejitve pošiljanja**, uveljavljene v storitvi.</span><span class="sxs-lookup"><span data-stu-id="6679f-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="6679f-104">Več informacij o teh omejitvah najdete [tukaj](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="6679f-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="6679f-105">Če želite preprečiti dostavo neželenih množičnih sporočil, so za vsakega uporabnika uporabljene **omejitve prejemnikov za vsa odhodna in notranja sporočila**.</span><span class="sxs-lookup"><span data-stu-id="6679f-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="6679f-106">Za vse inventarne številke je ta omejitev **10.000 prejemnikov na dan**.</span><span class="sxs-lookup"><span data-stu-id="6679f-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="6679f-107">Stranke, ki morajo poslati legitimna množična komercialna e-poštna sporočila (na primer novice za stranke), morajo uporabljati druge ponudnike, ki so namenjeni posebej za te storitve.</span><span class="sxs-lookup"><span data-stu-id="6679f-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="6679f-108">**Opomba**: Ko je dosežena omejitev prejemnikov, sporočil ni mogoče poslati iz nabiralnika, dokler število prejemnikov, ki so jim bila poslana sporočila v zadnjih 24 urah, ne pade pod omejitev.</span><span class="sxs-lookup"><span data-stu-id="6679f-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="6679f-109">Uporabnik do te točke ne bo mogel pošiljati sporočil.</span><span class="sxs-lookup"><span data-stu-id="6679f-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="6679f-110">Omejitev sporočil **30 sporočil na minuto** je uporabljena za vse inventarne številke.</span><span class="sxs-lookup"><span data-stu-id="6679f-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="6679f-111">To določa, koliko sporočil lahko uporabnik v določenem obdobju pošlje iz svojega računa Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="6679f-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="6679f-112">**Največje dovoljeno število prejemnikov v poljih »Za«, »Kp« in »Skp«** za eno e-poštno sporočilo v vseh inventarnih številkah je **1000 prejemnikov**.</span><span class="sxs-lookup"><span data-stu-id="6679f-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="6679f-113">To omejitev lahko prilagodite [tukaj](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="6679f-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
