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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977454"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="ca6aa-102">DLP ne deluje po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="ca6aa-102">DLP not working as expected</span></span>

<span data-ttu-id="ca6aa-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="ca6aa-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="ca6aa-104">**Nastavitev DLP**</span><span class="sxs-lookup"><span data-stu-id="ca6aa-104">**Setting up DLP**</span></span>

<span data-ttu-id="ca6aa-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** v officeu 365 ne deluje po pričakovanjih?</span><span class="sxs-lookup"><span data-stu-id="ca6aa-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="ca6aa-106">Če je tako, se prepričajte, da je **pravilnik DLP** pravilno nastavljen in da podatki vsebujejo tisto, kar išče **pravilnik DLP** , ko se ovrednoti.</span><span class="sxs-lookup"><span data-stu-id="ca6aa-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="ca6aa-107">Pravilniki DLP omogočajo prepoznavanje in zaščito občutljivih informacij v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="ca6aa-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="ca6aa-108">Če želite nastaviti pravilnike DLP, uporabite informacije [tukaj](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="ca6aa-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="ca6aa-109">**Katere politike DLP iščejo**</span><span class="sxs-lookup"><span data-stu-id="ca6aa-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="ca6aa-110">Pri uporabi **vgrajenih občutljivih vrst informacij** v središču Office 365 varnost in skladnost center, pravilniki DLP pri odkrivanju teh občutljivih tipov iščejo določene vzorce in elemente.</span><span class="sxs-lookup"><span data-stu-id="ca6aa-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="ca6aa-111">**Vgrajene vrste občutljivih informacij**</span><span class="sxs-lookup"><span data-stu-id="ca6aa-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="ca6aa-112">Če želite več informacij o vgrajenih vrstah občutljivih in o tem, kaj je videti v pravilniku o DLP pri odkrivanju občutljive vrste, glejte: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="ca6aa-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="ca6aa-113">**Vrste občutljivih informacij po meri**</span><span class="sxs-lookup"><span data-stu-id="ca6aa-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="ca6aa-114">Če poskušate ustvariti občutljive vrste informacij po meri, uporabite ta članek za informacije o tem, kako ustvariti občutljivo vrsto po meri: [ustvarite vrsto občutljive informacije po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="ca6aa-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="ca6aa-115">**Preskusite pravilnik DLP**</span><span class="sxs-lookup"><span data-stu-id="ca6aa-115">**Test a DLP policy**</span></span>

<span data-ttu-id="ca6aa-116">Če želite podatke preskusiti z vgrajenim ali po meri občutljivim informacijskim tipom, uporabite možnost **Vrsta preskusa** pod **razvrstitvami** > **občutljivih vrst**informacij.</span><span class="sxs-lookup"><span data-stu-id="ca6aa-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="ca6aa-117">Če želite več informacij, glejte [preizkušanje občutljivih vrst informacij po meri](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="ca6aa-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="ca6aa-118">**Poročila**</span><span class="sxs-lookup"><span data-stu-id="ca6aa-118">**Reports**</span></span>
  
- <span data-ttu-id="ca6aa-119">Pridobite občutljive vpoglede podatkov s [poročili DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="ca6aa-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="ca6aa-120">Oglejte si posebne podrobnosti dogodka s [poročilom o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="ca6aa-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
