---
title: Iskanje v SharePointovem spletu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044059"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="293fb-102">Vsebina, ki se plazi in indeksira v SharePoint online</span><span class="sxs-lookup"><span data-stu-id="293fb-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="293fb-103">Vsebino je treba preiskati in dodati v indeks iskanja za uporabnike, da najdejo tisto, kar iščejo v SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="293fb-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="293fb-104">Vsebina je samodejno preiskana na podlagi vnaprej določenega razporeda iskanja po vsebini (razporeda iskanja po vsebini ni mogoče spremeniti).</span><span class="sxs-lookup"><span data-stu-id="293fb-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="293fb-105">Iskalnik pobere vsebino, ki se je od zadnjega iskanja po vsebini spremenila, in posodobi indeks.</span><span class="sxs-lookup"><span data-stu-id="293fb-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="293fb-106">Če želite zagotoviti, da je vsebina preiskana in je indeks posodobljen, upoštevajte naslednje:</span><span class="sxs-lookup"><span data-stu-id="293fb-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="293fb-107">Prepričajte se, da je vsebina mogoče najti tako, [da se vsebina spletnega mesta omogoči iskanje](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="293fb-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="293fb-108">Ko ste spremenili upravljano lastnost ali ko ste spremenili preslikavo preiskanih in vodenih lastnosti, je treba mesto ponovno preiskati, preden se bodo spremembe odražale v indeksu iskanja.</span><span class="sxs-lookup"><span data-stu-id="293fb-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="293fb-109">Ker so vaše spremembe narejene v iskalni shemi in ne na dejanskem mestu, iskalnik ne bo samodejno ponovno indeksira mesta.</span><span class="sxs-lookup"><span data-stu-id="293fb-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="293fb-110">Če želite več informacij, glejte [ročno iskanje po vsebini in vnovično indeksiranje spletnega mesta, knjižnice ali seznama](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="293fb-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="293fb-111">Počakajte vsaj 24 ur po tem, ko ročno zahtevate iskanje po vsebini in celoten ponovni indeks, da preverite, ali še vedno naletite na težavo.</span><span class="sxs-lookup"><span data-stu-id="293fb-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="293fb-112">Če je minilo več kot 24 ur od začetka iskanja po vsebini in polnem ponovnem indeksu, prosimo, prijavite primer podpore.</span><span class="sxs-lookup"><span data-stu-id="293fb-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="293fb-113">V mnogih primerih že delamo na rešitvi.</span><span class="sxs-lookup"><span data-stu-id="293fb-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="293fb-114">Prosimo, dajte nam vsaj 24 ur, da dokončate rešitev.</span><span class="sxs-lookup"><span data-stu-id="293fb-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="293fb-115">Če je bilo mesto, dokument (knjižnica) ali seznam izbrisan in še vedno kaže v rezultatih iskanja, morajo uporabniki prejeti **napako 404 datoteka ni bilo mogoče najti** , ko poskušate dostopati do nje.</span><span class="sxs-lookup"><span data-stu-id="293fb-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="293fb-116">To vprašanje bi bilo treba prijaviti kot podporni primer za nadaljnjo preiskavo.</span><span class="sxs-lookup"><span data-stu-id="293fb-116">This issue should be logged as a support case for further investigation.</span></span> 



