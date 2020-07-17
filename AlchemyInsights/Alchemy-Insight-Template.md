---
title: isto kot filename je najprimernejši
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750986"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="da86c-102">"Zahtevana alkimija header H1, H2's ne dela."</span><span class="sxs-lookup"><span data-stu-id="da86c-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="da86c-103">Najboljše prakse in smernice za authoring Alchemy:</span><span class="sxs-lookup"><span data-stu-id="da86c-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="da86c-104">**Ne gnezdijo Alchemy Insights v mapah**-to bo prekinil URL strukturo.</span><span class="sxs-lookup"><span data-stu-id="da86c-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="da86c-105">Iščemo to.</span><span class="sxs-lookup"><span data-stu-id="da86c-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="da86c-106">Datoteke v mapi **Alchemyinsights** morajo imeti male imena datotek z vezaji za presledke ex.</span><span class="sxs-lookup"><span data-stu-id="da86c-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="da86c-107">***kako-v-usposobiti-pravda-počakaj***.</span><span class="sxs-lookup"><span data-stu-id="da86c-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="da86c-108">Vključite ID pravila ali ID vedra iz [portala Alchemy partner](https://alchemyportal.azurewebsites.net) v polje po meri MS.</span><span class="sxs-lookup"><span data-stu-id="da86c-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="da86c-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="da86c-109">ex.</span></span> <span data-ttu-id="da86c-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="da86c-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="da86c-111">Uporabite preostale metapodatke na vrhu te datoteke kot predlogo.</span><span class="sxs-lookup"><span data-stu-id="da86c-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="da86c-112">Na [portalu Alchemy partner](https://alchemyportal.azurewebsites.net), pomaknite navzdol do oddelka **Customer vpogled naslov:** in uporabite, da kot izhodišče za vaše h1 naslov za vpogled.</span><span class="sxs-lookup"><span data-stu-id="da86c-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="da86c-113">Alchemy Insights mora imeti samo en H1 na vrhu ali pa bo prekinil v proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="da86c-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="da86c-114">H2s ne postanejo tako uporabljajo **krepko** ali druge konvencije, da pomeni ločene oddelke.</span><span class="sxs-lookup"><span data-stu-id="da86c-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="da86c-115">Nato izpolnite besedilo telesa z uporabo osnutka gradiva v razdelku vpogled v stranke na strani pravila Alchemy</span><span class="sxs-lookup"><span data-stu-id="da86c-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="da86c-116">Označeni seznami so v redu</span><span class="sxs-lookup"><span data-stu-id="da86c-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="da86c-117">Oštevilčeni seznami preveč</span><span class="sxs-lookup"><span data-stu-id="da86c-117">Numbered lists too</span></span>
    1. <span data-ttu-id="da86c-118">**Krepko** in *Ležeče* so-ok</span><span class="sxs-lookup"><span data-stu-id="da86c-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="da86c-119">Povezave morajo biti vedno bodisi **"povezave do spleta"/zunanje** ali **Deep-povezave do elementov UI**, ne notranjih povezav.</span><span class="sxs-lookup"><span data-stu-id="da86c-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="da86c-120">Slike niso uradno podprte v tem trenutku, vendar je na časovnem načrtu.</span><span class="sxs-lookup"><span data-stu-id="da86c-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="da86c-121">In to je že malo predolgo.</span><span class="sxs-lookup"><span data-stu-id="da86c-121">And this is really already a bit too long.</span></span> <span data-ttu-id="da86c-122">Najboljša praksa je približno 400 znakov---------------------------------</span><span class="sxs-lookup"><span data-stu-id="da86c-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="da86c-123">Ko je vsebina pripravljena, jo povlecite v podružnico v živo.</span><span class="sxs-lookup"><span data-stu-id="da86c-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="da86c-124">Nato pojdite na [portal Alchemy partner](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje URL.</span><span class="sxs-lookup"><span data-stu-id="da86c-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 