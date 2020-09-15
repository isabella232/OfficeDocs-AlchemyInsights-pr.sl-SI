---
title: enako kot ime datoteke je najboljše
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664150"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="03af6-102">"Zahtevani Alchemy header H1, H2's ne delujejo."</span><span class="sxs-lookup"><span data-stu-id="03af6-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="03af6-103">Najboljše prakse in smernice za ustvarjanje avtorjev alkimije:</span><span class="sxs-lookup"><span data-stu-id="03af6-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="03af6-104">**Do not Nest vpogledov v mape**– to bo prekinilo strukturo URL-ja.</span><span class="sxs-lookup"><span data-stu-id="03af6-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="03af6-105">Poskušamo popraviti to.</span><span class="sxs-lookup"><span data-stu-id="03af6-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="03af6-106">Datoteke v mapi **AlchemyInsights** morajo imeti male datoteke z vezaji za presledke ex.</span><span class="sxs-lookup"><span data-stu-id="03af6-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="03af6-107">***navodila za omogočanje uporabe v sporu – pridržite***.</span><span class="sxs-lookup"><span data-stu-id="03af6-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="03af6-108">Vključite ID pravila ali ID vedra na [partnerskem portalu Alchemy](https://alchemyportal.azurewebsites.net) v polju MS. po meri.</span><span class="sxs-lookup"><span data-stu-id="03af6-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="03af6-109">ex.</span><span class="sxs-lookup"><span data-stu-id="03af6-109">ex.</span></span> <span data-ttu-id="03af6-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="03af6-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="03af6-111">Uporabite preostala metapodatka na vrhu te datoteke kot predlogo.</span><span class="sxs-lookup"><span data-stu-id="03af6-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="03af6-112">V [partnerskem portalu Alchemy](https://alchemyportal.azurewebsites.net)se pomaknite do razdelka» **naslov stranke vpogleda «:** in uporabite to kot izhodišče za vaš naslov H1 za vpogled.</span><span class="sxs-lookup"><span data-stu-id="03af6-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="03af6-113">V programu Alchemy vpogledi morajo biti le en H1 na vrhu ali pa bodo vdrli v proizvodnjo.</span><span class="sxs-lookup"><span data-stu-id="03af6-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="03af6-114">H2s ne omogoča uporabe **krepkih** ali drugih konvencij, da bi označili ločene odseke.</span><span class="sxs-lookup"><span data-stu-id="03af6-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="03af6-115">Nato vnesite besedilo v telo z uporabo osnutka gradiva v razdelku» vpogledi v stranke «na strani» pravilo Alchemy «</span><span class="sxs-lookup"><span data-stu-id="03af6-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="03af6-116">Označeni seznami so Fini</span><span class="sxs-lookup"><span data-stu-id="03af6-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="03af6-117">Tudi oštevilčeni seznami</span><span class="sxs-lookup"><span data-stu-id="03af6-117">Numbered lists too</span></span>
    1. <span data-ttu-id="03af6-118">**Krepko** in *Ležeče* so a-ok</span><span class="sxs-lookup"><span data-stu-id="03af6-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="03af6-119">Povezave bi morale biti vedno **» povezave do spleta «/External** ali **Deep povezave do elementov uporabniškega vmesnika**in ne notranjih povezav.</span><span class="sxs-lookup"><span data-stu-id="03af6-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="03af6-120">Slike trenutno niso uradno podprte, vendar je to v načrtu.</span><span class="sxs-lookup"><span data-stu-id="03af6-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="03af6-121">In to je res že nekoliko predolgo.</span><span class="sxs-lookup"><span data-stu-id="03af6-121">And this is really already a bit too long.</span></span> <span data-ttu-id="03af6-122">Najboljša praksa je približno 400 znakov---------------------------------</span><span class="sxs-lookup"><span data-stu-id="03af6-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="03af6-123">Ko je vaša vsebina pripravljena, jo potegnite v živo vejo.</span><span class="sxs-lookup"><span data-stu-id="03af6-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="03af6-124">Nato pojdite na portal za [partnerje Alchemy](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje URL.</span><span class="sxs-lookup"><span data-stu-id="03af6-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 