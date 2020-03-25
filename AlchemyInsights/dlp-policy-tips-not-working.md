---
title: DLP Policy Nasveti ne delujejo
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932602"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="a5a2c-102">Vprašanja za namig pravilnika DLP</span><span class="sxs-lookup"><span data-stu-id="a5a2c-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="a5a2c-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a5a2c-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a5a2c-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a5a2c-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a5a2c-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a5a2c-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a5a2c-109">**Namigi pravilnika DLP**</span><span class="sxs-lookup"><span data-stu-id="a5a2c-109">**DLP policy tips**</span></span>

<span data-ttu-id="a5a2c-110">Pri uporabi **pravilnikov DLP**so uporabniki lahko obveščeni o kršitvi pravilnika z **namigi pravilnika**.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="a5a2c-111">Skrbniki lahko konfigurirajo nasvete pravilnika za prikaz med preskušanjem pravilnika DLP ali ko je pravilnik v polnem načinu izvrševanja.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="a5a2c-112">Če želite konfigurirati nasvete pravilnika za pravilnik DLP v središču za varnost in skladnost v celotnem načinu izvrševanja, naredite to:</span><span class="sxs-lookup"><span data-stu-id="a5a2c-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="a5a2c-113">Zagotovite, da so bili namigi pravilnika **omogočeni** v pravilu DLP z uporabo korakov [tukaj](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="a5a2c-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="a5a2c-114">Zagotovite, da se **vsebina ujema** s tem, kar je **potrebno** za sprožitev pravila, ki je opisan v tem članku [tukaj](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="a5a2c-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="a5a2c-115">Nasveti politike prikazujejo v obeh OWA in Outlook.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="a5a2c-116">Vendar, ko uporabljate **Outlook 2013 ali novejši**, so namigi pravilnika prikazani le pod določenimi pogoji.</span><span class="sxs-lookup"><span data-stu-id="a5a2c-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="a5a2c-117">Ti pogoji so navedeni tukaj: [podprti pogoji za Outlook 2013 ali novejše za prikazovanje nasvetov pravilnika](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="a5a2c-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="a5a2c-118">Če želite dodatne informacije o nasvetih pravilnika DLP, glejte: [Pokaži nasvete pravilnika za pravilnike DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="a5a2c-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  