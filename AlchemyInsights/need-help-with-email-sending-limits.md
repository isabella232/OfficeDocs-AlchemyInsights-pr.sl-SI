---
title: Potrebujete pomoč pri omejitvah pošiljanja e-pošte?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358358"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="1fd89-102">Potrebujete pomoč pri omejitvah pošiljanja e-pošte?</span><span class="sxs-lookup"><span data-stu-id="1fd89-102">Need help with email sending limits?</span></span>

<span data-ttu-id="1fd89-103">Spodaj je **po-design omejitve pošiljanja** izvrši v službi.</span><span class="sxs-lookup"><span data-stu-id="1fd89-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="1fd89-104">Več informacij o teh omejitvah je [tukaj](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)dokumentirano.</span><span class="sxs-lookup"><span data-stu-id="1fd89-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="1fd89-105">Če želite preprečiti dostavo nenaročenih množičnih sporočil, **za vsa odhodna in notranja sporočila uporabimo omejitve števila prejemnikov**po uporabnikih.</span><span class="sxs-lookup"><span data-stu-id="1fd89-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="1fd89-106">Čez vsi SKUs, to višek je **10.000 sprejemnik po dan**.</span><span class="sxs-lookup"><span data-stu-id="1fd89-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="1fd89-107">Stranke, ki morajo poslati legitimno komercialno e-poštno sporočilo (na primer novice o strankah), morajo uporabljati ponudnike neodvisnih ponudnikov, ki so specializirani za te storitve.</span><span class="sxs-lookup"><span data-stu-id="1fd89-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="1fd89-108">**Opomba**: ko je dosežena omejitev števila prejemnikov, sporočil ni mogoče pošiljati iz nabiralnika, dokler število prejemnikov, poslanih sporočilom v zadnjih 24 urah, pade pod mejo.</span><span class="sxs-lookup"><span data-stu-id="1fd89-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="1fd89-109">Uporabnik ne bo mogel pošiljati sporočil do te točke.</span><span class="sxs-lookup"><span data-stu-id="1fd89-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="1fd89-110">Omejitev hitrosti sporočila **30 sporočil na minuto** se uporablja v vseh SKUs.</span><span class="sxs-lookup"><span data-stu-id="1fd89-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="1fd89-111">To določa, koliko sporočil lahko uporabnik pošlje iz svojega računa Exchange Online v določenem obdobju.</span><span class="sxs-lookup"><span data-stu-id="1fd89-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="1fd89-112">**Največje število prejemnikov, dovoljenih v poljih za, CC in BCC** za eno e-poštno sporočilo, je v vseh skus **1000 prejemnikov**.</span><span class="sxs-lookup"><span data-stu-id="1fd89-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="1fd89-113">Če želite prilagoditi to omejitev, pojdite [tukaj](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="1fd89-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
