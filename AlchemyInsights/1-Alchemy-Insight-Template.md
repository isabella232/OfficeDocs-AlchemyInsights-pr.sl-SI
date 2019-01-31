---
title: 'enako kot ime datoteke, je najbolje [pravilo #-opis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 1bb1cb35f06e16a2dc85b7e2642b9fa0d203945e
ms.sourcegitcommit: b032c2ac45540b1eb5dd68a4ec7ce1a5d6922f0e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662946"
---
# <a name="required-customer-facing-h1-h2-doesnt-work"></a><span data-ttu-id="b2a96-102">Potrebna kupca sooča H1, H2, ne deluje</span><span class="sxs-lookup"><span data-stu-id="b2a96-102">Required Customer Facing H1, H2 doesn't work</span></span>
<span data-ttu-id="b2a96-103">Primer besedilo blokiranje - sledite tem navodilom:</span><span class="sxs-lookup"><span data-stu-id="b2a96-103">Example text block - follow these instructions:</span></span>

1. <span data-ttu-id="b2a96-104">Datoteke v mapi **AlchemyInsights** mora imeti pravilo ID in ime pravila iz [alkimije Partner portal](https://alchemyportal.azurewebsites.net) v ime datoteke.</span><span class="sxs-lookup"><span data-stu-id="b2a96-104">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="b2a96-p101">ex. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="b2a96-p101">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="b2a96-p102">Metapodatke na vrhu te datoteke uporabite kot predlogo. Nič drugega ni potrebno.</span><span class="sxs-lookup"><span data-stu-id="b2a96-p102">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="b2a96-109">[Alchemy Partner portal](https://alchemyportal.azurewebsites.net)pluti niz v oddelku **strank vpogled naslova:** in uporabo, ki kot začetno točko za vaš H1 naslov za vpogled.</span><span class="sxs-lookup"><span data-stu-id="b2a96-109">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="b2a96-p103">Alkimija vpogled mora imeti samo eno H1 na vrhu, ali bo prekinil v proizvodnji. H2s ne postanejo tako uporabo **krepko** ali drugih konvencij, da se označi ločenih odsekih.</span><span class="sxs-lookup"><span data-stu-id="b2a96-p103">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="b2a96-112">Nato izpolnite telesa besedila z uporabo osnutek material v razdelku strank vpogled Alchemy pravilo strani</span><span class="sxs-lookup"><span data-stu-id="b2a96-112">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="b2a96-113">Označeni seznami so v redu</span><span class="sxs-lookup"><span data-stu-id="b2a96-113">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="b2a96-114">Tudi oštevilčene sezname</span><span class="sxs-lookup"><span data-stu-id="b2a96-114">Numbered lists too</span></span>
    1. <span data-ttu-id="b2a96-115">**Krepko** in *Ležeče* so ok-</span><span class="sxs-lookup"><span data-stu-id="b2a96-115">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="b2a96-116">Povezave morajo biti vedno bodisi **"povezave do spletnih" / zunanje** ali **globoko povezav z elementi uporabniškega vmesnika**, ni notranjih povezav.</span><span class="sxs-lookup"><span data-stu-id="b2a96-116">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="b2a96-p104">In to je res že malo predolgo. Najboljše prakse je približno 400 znakov---</span><span class="sxs-lookup"><span data-stu-id="b2a96-p104">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="b2a96-p105">Ko vsebino, je pripravljen, potegnem v živo veja. Potem obiščite [alkimije Partner portal](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje url. Preverite, ali vpogled pregledali in objavila pravi, "da" in kliknite posodobitev pravilo. (To bo videti lepši v novi različici portala - sprošča kmalu.)</span><span class="sxs-lookup"><span data-stu-id="b2a96-p105">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. (This will look prettier in the new version of the portal - releasing soon.)</span></span>

![URL polje](media/for-content-team.PNG)

