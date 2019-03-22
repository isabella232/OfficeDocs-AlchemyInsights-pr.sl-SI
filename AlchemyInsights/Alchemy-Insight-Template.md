---
title: enako kot ime datoteke je najboljši
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 5555
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 68f743ee9c448565470815f8410cc6ce4b384bed
ms.sourcegitcommit: 0b6e9470c6b73616ba8bacef7010f739b7fac332
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/21/2019
ms.locfileid: "30742462"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="860b6-102">Zahteva alkimije glavo H1, H2 je ne dela.</span><span class="sxs-lookup"><span data-stu-id="860b6-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="860b6-103">Najboljše prakse in smernice za alkimijo authoring:</span><span class="sxs-lookup"><span data-stu-id="860b6-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="860b6-104">**Ne ugnezdite Alchemy vpogled v mapah**- to bo prekinil url strukture.</span><span class="sxs-lookup"><span data-stu-id="860b6-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="860b6-105">Iščemo v pritrjevanje to.</span><span class="sxs-lookup"><span data-stu-id="860b6-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="860b6-106">Datoteke v mapi **AlchemyInsights** morajo imeti male črke imena datotek z vezaji za prostore ex.</span><span class="sxs-lookup"><span data-stu-id="860b6-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="860b6-107">***kako-to-usposobiti--čakanje***.</span><span class="sxs-lookup"><span data-stu-id="860b6-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="860b6-108">Vključujejo ID pravilo ID ali vedro iz [alkimije Partner portal](https://alchemyportal.azurewebsites.net) na ms.custom področju.</span><span class="sxs-lookup"><span data-stu-id="860b6-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="860b6-109">ex.</span><span class="sxs-lookup"><span data-stu-id="860b6-109">ex.</span></span> <span data-ttu-id="860b6-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="860b6-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="860b6-111">Preostanek metapodatke na vrhu te datoteke uporabite kot predlogo.</span><span class="sxs-lookup"><span data-stu-id="860b6-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="860b6-112">[Alchemy Partner portal](https://alchemyportal.azurewebsites.net)pluti niz v oddelku **strank vpogled naslova:** in uporabo, ki kot začetno točko za vaš H1 naslov za vpogled.</span><span class="sxs-lookup"><span data-stu-id="860b6-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="860b6-113">Alkimija vpogled mora imeti samo eno H1 na vrhu, ali bo prekinil v proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="860b6-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="860b6-114">H2s ne postanejo tako uporabo **krepko** ali drugih konvencij, da se označi ločenih odsekih.</span><span class="sxs-lookup"><span data-stu-id="860b6-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="860b6-115">Nato izpolnite telesa besedila z uporabo osnutek material v razdelku strank vpogled Alchemy pravilo strani</span><span class="sxs-lookup"><span data-stu-id="860b6-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="860b6-116">Označeni seznami so v redu</span><span class="sxs-lookup"><span data-stu-id="860b6-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="860b6-117">Tudi oštevilčene sezname</span><span class="sxs-lookup"><span data-stu-id="860b6-117">Numbered lists too</span></span>
    1. <span data-ttu-id="860b6-118">**Krepko** in *Ležeče* so ok-</span><span class="sxs-lookup"><span data-stu-id="860b6-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="860b6-119">Povezave morajo biti vedno bodisi **"povezave do spletnih" / zunanje** ali **globoko povezav z elementi uporabniškega vmesnika**, ni notranjih povezav.</span><span class="sxs-lookup"><span data-stu-id="860b6-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="860b6-120">Slike ni uradno podprta v tem trenutku, vendar je na načrtu.</span><span class="sxs-lookup"><span data-stu-id="860b6-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="860b6-121">In to je res že malo predolgo.</span><span class="sxs-lookup"><span data-stu-id="860b6-121">And this is really already a bit too long.</span></span> <span data-ttu-id="860b6-122">Najboljše prakse je približno 400 znakov---</span><span class="sxs-lookup"><span data-stu-id="860b6-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="860b6-123">Ko vsebino, je pripravljen, potegnem v živo veja.</span><span class="sxs-lookup"><span data-stu-id="860b6-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="860b6-124">Potem obiščite [alkimije Partner portal](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje url.</span><span class="sxs-lookup"><span data-stu-id="860b6-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="860b6-125">M</span><span class="sxs-lookup"><span data-stu-id="860b6-125">M</span></span>