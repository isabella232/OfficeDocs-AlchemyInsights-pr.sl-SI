---
title: DLP ne deluje po pričakovanjih
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932638"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="c3eea-102">DLP ne deluje po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="c3eea-102">DLP not working as expected</span></span>

<span data-ttu-id="c3eea-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="c3eea-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c3eea-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="c3eea-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c3eea-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="c3eea-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c3eea-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="c3eea-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c3eea-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="c3eea-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c3eea-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="c3eea-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="c3eea-109">**Nastavitev DLP**</span><span class="sxs-lookup"><span data-stu-id="c3eea-109">**Setting up DLP**</span></span>

<span data-ttu-id="c3eea-110">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** v officeu 365 ne deluje po pričakovanjih?</span><span class="sxs-lookup"><span data-stu-id="c3eea-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="c3eea-111">Če je tako, se prepričajte, da je **pravilnik DLP** pravilno nastavljen in da podatki vsebujejo tisto, kar išče **pravilnik DLP** , ko se ovrednoti.</span><span class="sxs-lookup"><span data-stu-id="c3eea-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="c3eea-112">Pravilniki DLP omogočajo prepoznavanje in zaščito občutljivih informacij v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="c3eea-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="c3eea-113">Če želite nastaviti pravilnike DLP, uporabite informacije [tukaj](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="c3eea-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="c3eea-114">**Katere politike DLP iščejo**</span><span class="sxs-lookup"><span data-stu-id="c3eea-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="c3eea-115">Pri uporabi **vgrajenih občutljivih vrst informacij** v središču Office 365 varnost in skladnost center, pravilniki DLP pri odkrivanju teh občutljivih tipov iščejo določene vzorce in elemente.</span><span class="sxs-lookup"><span data-stu-id="c3eea-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="c3eea-116">**Vgrajene vrste občutljivih informacij**</span><span class="sxs-lookup"><span data-stu-id="c3eea-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="c3eea-117">Če želite več informacij o vgrajenih vrstah občutljivih in o tem, kaj je videti v pravilniku o DLP pri odkrivanju občutljive vrste, glejte: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="c3eea-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="c3eea-118">**Vrste občutljivih informacij po meri**</span><span class="sxs-lookup"><span data-stu-id="c3eea-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="c3eea-119">Če poskušate ustvariti občutljive vrste informacij po meri, uporabite ta članek za informacije o tem, kako ustvariti občutljivo vrsto po meri: [ustvarite vrsto občutljive informacije po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c3eea-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="c3eea-120">**Preskusite pravilnik DLP**</span><span class="sxs-lookup"><span data-stu-id="c3eea-120">**Test a DLP policy**</span></span>

<span data-ttu-id="c3eea-121">Če želite podatke preskusiti z vgrajenim ali po meri občutljivim informacijskim tipom, uporabite možnost **Vrsta preskusa** pod **razvrstitvami** > **občutljivih vrst**informacij.</span><span class="sxs-lookup"><span data-stu-id="c3eea-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="c3eea-122">Če želite več informacij, glejte [preizkušanje občutljivih vrst informacij po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="c3eea-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="c3eea-123">**Poročila**</span><span class="sxs-lookup"><span data-stu-id="c3eea-123">**Reports**</span></span>
  
- <span data-ttu-id="c3eea-124">Pridobite občutljive vpoglede podatkov s [poročili DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="c3eea-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="c3eea-125">Oglejte si posebne podrobnosti dogodka s [poročilom o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="c3eea-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
