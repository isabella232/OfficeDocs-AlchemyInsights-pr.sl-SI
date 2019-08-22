---
title: Išči v SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507647"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="64872-102">Vsebine iskanje in indeksiranje v SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="64872-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="64872-103">Vsebina mora preiskati in doda v kazalo iskanja za uporabnike, da bi našli tisto, kar oni iščejo v SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="64872-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="64872-104">Samodejno vsebini temelji na vnaprej določenih iskanja razpored (razpored iskanja po vsebini ni mogoče spremeniti).</span><span class="sxs-lookup"><span data-stu-id="64872-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="64872-105">Iskalnik dvigne vsebine, ki se je spremenilo od zadnjega iskanja po vsebini in posodobi kazalo.</span><span class="sxs-lookup"><span data-stu-id="64872-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="64872-106">Za zagotovitev vsebini in je kazalo posodobljeno, upoštevajte naslednje:</span><span class="sxs-lookup"><span data-stu-id="64872-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="64872-107">Poskrbite, da vsebine najdete tako, [da vsebino strani iskanje](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="64872-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="64872-108">Ko spremenite upravljane lastnosti, ali ko ste spremenili kartiranje obiskal in upravljati lastnosti, mesta morajo biti ponovno obiskal, preden se spremembe odrazijo v kazalu iskanja.</span><span class="sxs-lookup"><span data-stu-id="64872-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="64872-109">Ker so vaše spremembe v shemi iskanje, in ne do dejanskih strani, iskalnik ne bo samodejno ponovno indeksiranje strani.</span><span class="sxs-lookup"><span data-stu-id="64872-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="64872-110">Za več informacij, glejte [zahteva ročno iskanje in ponovno indeksiranje strani, knjižnico ali seznam](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="64872-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="64872-111">Počakajte vsaj 24 ur po ročno zahteva iskanja in poln ponovnega indeksiranja, da vidim, če ste še vedno prihaja do težave.</span><span class="sxs-lookup"><span data-stu-id="64872-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="64872-112">Če več kot 24 ur je minilo, odkar si začel plazijo in poln ponovnega indeksiranja, se prijavite na primer podporo.</span><span class="sxs-lookup"><span data-stu-id="64872-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="64872-113">V mnogih primerih, že delamo na rešitev.</span><span class="sxs-lookup"><span data-stu-id="64872-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="64872-114">Prosimo, da nam vsaj 24 ur za dokončanje rešitev.</span><span class="sxs-lookup"><span data-stu-id="64872-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="64872-115">Če stran, dokument (knjižnice), ali seznam je bil izbrisan in še vedno prikazuje v rezultatih iskanja, uporabnik should sprejemati **Napaka 404 datoteke ni mogoče najti** čas težaven v postranski to.</span><span class="sxs-lookup"><span data-stu-id="64872-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="64872-116">To vprašanje, naj zapišejo kot primer podporo za dodatne preiskave.</span><span class="sxs-lookup"><span data-stu-id="64872-116">This issue should be logged as a support case for further investigation.</span></span> 



