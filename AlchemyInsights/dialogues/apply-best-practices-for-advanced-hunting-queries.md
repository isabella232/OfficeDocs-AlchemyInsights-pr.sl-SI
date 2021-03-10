---
title: Uporaba najboljših praks za napredne poizvedbe za lov
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696083"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="4e576-102">Uporaba najboljših praks za napredne poizvedbe za lov</span><span class="sxs-lookup"><span data-stu-id="4e576-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="4e576-103">Če želite hitreje dobiti rezultate in se izogniti časovnim presledkom med izvajanjem zapletenih poizvedb, uporabite te najboljše prakse:</span><span class="sxs-lookup"><span data-stu-id="4e576-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="4e576-104">Ko poskušate uporabiti nove poizvedbe, vedno uporabite omejitev, da se izognete zelo velikim naborom rezultatov.</span><span class="sxs-lookup"><span data-stu-id="4e576-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="4e576-105">Uporabite tudi, `count` Če želite opraviti začetno oceno velikosti nabora rezultatov.</span><span class="sxs-lookup"><span data-stu-id="4e576-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="4e576-106">Najprej uporabite časovne filtre.</span><span class="sxs-lookup"><span data-stu-id="4e576-106">Use time filters first.</span></span> <span data-ttu-id="4e576-107">V idealnem primeru omejite svoje poizvedbe na sedem dni.</span><span class="sxs-lookup"><span data-stu-id="4e576-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="4e576-108">Na začetku poizvedbe takoj za časovnim filtrom dodajte filtre, ki naj bi odstranili večino podatkov.</span><span class="sxs-lookup"><span data-stu-id="4e576-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="4e576-109">Ko iščete polne žetone, uporabite `has` operator namesto `contains` .</span><span class="sxs-lookup"><span data-stu-id="4e576-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="4e576-110">Zaženite iskanje v določenem stolpcu in ne v vseh stolpcih.</span><span class="sxs-lookup"><span data-stu-id="4e576-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="4e576-111">Ko se pridružite tabelam, najprej določite tabelo z manj vrsticami.</span><span class="sxs-lookup"><span data-stu-id="4e576-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="4e576-112">`project` le potrebne stolpce iz tabel, ki ste jih priključili.</span><span class="sxs-lookup"><span data-stu-id="4e576-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="4e576-113">Če želite izvedeti več, glejte [napredne prakse za lov](https://go.microsoft.com/fwlink/?linkid=2144812)na iskanje.</span><span class="sxs-lookup"><span data-stu-id="4e576-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
