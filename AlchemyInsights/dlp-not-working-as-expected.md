---
title: DLP ne deluje po pričakovanjih
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679709"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="f6685-102">DLP ne deluje po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="f6685-102">DLP not working as expected</span></span>

<span data-ttu-id="f6685-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="f6685-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="f6685-104">**Nastavitev DLP**</span><span class="sxs-lookup"><span data-stu-id="f6685-104">**Setting up DLP**</span></span>

<span data-ttu-id="f6685-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** v sistemu Office 365 ne deluje po pričakovanjih?</span><span class="sxs-lookup"><span data-stu-id="f6685-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="f6685-106">V tem primeru preverite, ali je **pravilnik za DLP** pravilno nastavljen in da podatki vsebujejo, kaj išče **pravilnik DLP** , ko ga ocenjujete.</span><span class="sxs-lookup"><span data-stu-id="f6685-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="f6685-107">Pravilniki DLP omogočajo prepoznavanje in zaščito občutljivih informacij v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="f6685-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="f6685-108">Če želite nastaviti pravilnike za DLP, uporabite informacije [tukaj](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="f6685-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="f6685-109">**Katere pravilnike za DLP iščejo**</span><span class="sxs-lookup"><span data-stu-id="f6685-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="f6685-110">Ko uporabljate **vgrajene občutljive vrste podatkov** v centrih za varnost in skladnost, pravilniki DLP iščejo določene vzorce in elemente pri odkrivanju teh občutljivih vrst.</span><span class="sxs-lookup"><span data-stu-id="f6685-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="f6685-111">**Vgrajene občutljive vrste informacij**</span><span class="sxs-lookup"><span data-stu-id="f6685-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="f6685-112">Če želite več informacij o vgrajenih občutljivih vrstah in o tem, kaj išče pravilnik za DLP pri odkrivanju občutljive vrste, glejte: [Kaj iščejo vrste občutljivih informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="f6685-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="f6685-113">**Vrste občutljivih podatkov po meri**</span><span class="sxs-lookup"><span data-stu-id="f6685-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="f6685-114">Če želite ustvariti občutljive vrste podatkov po meri, uporabite ta članek, če želite informacije o tem, kako ustvariti vrsto občutljivega po meri: [ustvarite vrsto občutljivih podatkov po meri](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="f6685-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="f6685-115">**Preskus pravilnika za DLP**</span><span class="sxs-lookup"><span data-stu-id="f6685-115">**Test a DLP policy**</span></span>

<span data-ttu-id="f6685-116">Če želite preskusiti podatke z vgrajenim tipom ali občutljivo vrsto podatkov po meri, uporabite možnost» **Vrsta preskusa** «v razdelku **razvrstitve**  >  **občutljive vrste informacij**.</span><span class="sxs-lookup"><span data-stu-id="f6685-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="f6685-117">Če želite več informacij, glejte [preskušanje vrst občutljivih podatkov po meri](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="f6685-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="f6685-118">**Poročila**</span><span class="sxs-lookup"><span data-stu-id="f6685-118">**Reports**</span></span>
  
- <span data-ttu-id="f6685-119">Pridobite občutljive vpoglede podatkov s [poročili DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="f6685-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="f6685-120">Oglejte si natančne podrobnosti dogodka z [poročilom o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="f6685-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
