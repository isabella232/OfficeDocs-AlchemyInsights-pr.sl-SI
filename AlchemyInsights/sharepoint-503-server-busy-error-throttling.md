---
title: SharePoint online Throttling
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931242"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="170ac-102">SharePoint online Throttling</span><span class="sxs-lookup"><span data-stu-id="170ac-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="170ac-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="170ac-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="170ac-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="170ac-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="170ac-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="170ac-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="170ac-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="170ac-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="170ac-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="170ac-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="170ac-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="170ac-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="170ac-109">**503 strežnik je zaseden napaka**</span><span class="sxs-lookup"><span data-stu-id="170ac-109">**503 server is busy error**</span></span>

<span data-ttu-id="170ac-110">Uporabnik maj sprejemati a 503 pomočnik je zaposlen zmota čas poskus v pluti v SharePoint ali OneDrive položaj.</span><span class="sxs-lookup"><span data-stu-id="170ac-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="170ac-111">To napako lahko povzroči zadavljenje znotraj storitve SharePoint.</span><span class="sxs-lookup"><span data-stu-id="170ac-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="170ac-112">SharePoint online uporablja zadaviti za ohranjanje optimalne učinkovitosti in zanesljivosti storitve SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="170ac-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="170ac-113">Throttling omejuje število uporabniških dejanj ali sočasnih klicev (po skriptu ali kodi), da se prepreči prekomerna uporaba virov.</span><span class="sxs-lookup"><span data-stu-id="170ac-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="170ac-114">Za več informacij o zadaviti glej, [ne pridobivanje zadaviti ali blokiran v SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="170ac-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="170ac-115">Če menite, da ta napaka ni povezana z Throttling, lahko preverite, ali je aktivno vzdrževanje, ki se pojavljajo na vašem najemniku z navigacijo do [centra za sporočila](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="170ac-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="170ac-116">Slednjič, zavarovati vi kratek obisk [usluga zdravje](https://portal.office.com/adminportal/home#/servicehealth) stran v ček zakaj poljuben Advisories/nezgoda to maj obstati dogodek.</span><span class="sxs-lookup"><span data-stu-id="170ac-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

