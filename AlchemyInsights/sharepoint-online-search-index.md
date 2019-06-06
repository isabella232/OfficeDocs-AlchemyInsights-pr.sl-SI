---
title: Upravljanje iskanja slovarji v SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736068"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="b21c2-102">Išči v SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b21c2-102">Search in SharePoint Online</span></span>

<span data-ttu-id="b21c2-103">Vsebina mora preiskati in doda v kazalo iskanja za uporabnike, da bi našli tisto, kar oni iščejo v SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="b21c2-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="b21c2-104">Samodejno vsebini temelji na vnaprej določenih iskanja razpored (razpored iskanja po vsebini ni mogoče spremeniti).</span><span class="sxs-lookup"><span data-stu-id="b21c2-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="b21c2-105">Iskalnik dvigne vsebine, ki se je spremenilo od zadnjega iskanja po vsebini in posodobi kazalo.</span><span class="sxs-lookup"><span data-stu-id="b21c2-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="b21c2-106">Za zagotovitev vsebini in je kazalo posodobljeno, sledite spodnjim korakom.</span><span class="sxs-lookup"><span data-stu-id="b21c2-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="b21c2-107">Poskrbite, da vsebine najdete tako, da vsebino strani iskanje.</span><span class="sxs-lookup"><span data-stu-id="b21c2-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="b21c2-108">Za več informacij, glejte [Omogoči vsebino na strani, da je mogoče iskati](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b21c2-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="b21c2-109">Ko spremenite upravljane lastnosti, ali ko ste spremenili kartiranje obiskal in upravljati lastnosti, mesta morajo biti ponovno obiskal, preden se spremembe odrazijo v kazalu iskanja.</span><span class="sxs-lookup"><span data-stu-id="b21c2-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="b21c2-110">Ker so vaše spremembe v shemi iskanje, in ne do dejanskih strani, iskalnik ne bo samodejno ponovno indeksiranje strani.</span><span class="sxs-lookup"><span data-stu-id="b21c2-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="b21c2-111">Za več informacij, glejte [zahteva ročno iskanje in ponovno indeksiranje strani, knjižnico ali seznam](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="b21c2-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="b21c2-112">Počakajte vsaj 24 ur po ročno zahteva iskanja in poln ponovnega indeksiranja, da vidim, če ste še vedno prihaja do težave.</span><span class="sxs-lookup"><span data-stu-id="b21c2-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="b21c2-113">Če več kot 24 ur je minilo, odkar si začel plazijo in poln ponovnega indeksiranja, se prijavite na primer podporo.</span><span class="sxs-lookup"><span data-stu-id="b21c2-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="b21c2-114">V mnogih primerih, že delamo na rešitev.</span><span class="sxs-lookup"><span data-stu-id="b21c2-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b21c2-115">Prosimo, da nam vsaj 24 ur za dokončanje rešitev.</span><span class="sxs-lookup"><span data-stu-id="b21c2-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="b21c2-116">**Pomembno**: če stran, dokument (knjižnice) ali seznam je bil izbrisan in še vedno prikazuje v rezultatih iskanja, uporabnik should sprejemati je napaka 404 datoteke ni mogoče najti čas težaven v postranski.</span><span class="sxs-lookup"><span data-stu-id="b21c2-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="b21c2-117">To vprašanje, naj zapišejo kot primer podporo za dodatne preiskave.</span><span class="sxs-lookup"><span data-stu-id="b21c2-117">This issue should be logged as a support case for further investigation.</span></span> 



