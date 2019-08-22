---
title: DLP, ki ne deluje po pričakovanjih
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
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530311"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="c9c03-102">DLP, ki ne deluje po pričakovanjih</span><span class="sxs-lookup"><span data-stu-id="c9c03-102">DLP not working as expected</span></span>

<span data-ttu-id="c9c03-103">Ali imate težave s **Podatki Loss preprečevanje (DLP)** v Office 365, ki ne deluje po pričakovanjih?</span><span class="sxs-lookup"><span data-stu-id="c9c03-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="c9c03-104">Če je tako, se prepričajte, da vaš **DLP politike** pravilno nastavljen, in da podatki vsebujejo kaj **DLP politika** išče, ko to ocenjujejo.</span><span class="sxs-lookup"><span data-stu-id="c9c03-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="c9c03-105">**Nastavljanje DLP**</span><span class="sxs-lookup"><span data-stu-id="c9c03-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="c9c03-106">DLP politike omogoča prepoznavanje in zaščito občutljivih podatkov v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="c9c03-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="c9c03-107">Setup DLP politike, uporabljajo informacije [tukaj](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="c9c03-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="c9c03-108">**Kaj DLP pravila iskati**</span><span class="sxs-lookup"><span data-stu-id="c9c03-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="c9c03-109">Ko uporabljate **vgrajeno občutljivih podatkov vrste** Office 365 varnost in skladnost center, DLP pravila iskati določene vzorce in elementi pri odkrivanju teh občutljivih vrst.</span><span class="sxs-lookup"><span data-stu-id="c9c03-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="c9c03-110">**Vgrajeno občutljivih podatkov vrste**</span><span class="sxs-lookup"><span data-stu-id="c9c03-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="c9c03-111">Informacije o vgrajeni občutljivih vrst in kaj DLP politika išče, ko zazna občutljive vrste, glejte: [iskati kakšne vrste občutljivih informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="c9c03-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="c9c03-112">**Vrste po meri občutljivih informacij**</span><span class="sxs-lookup"><span data-stu-id="c9c03-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="c9c03-113">Če želite ustvariti vrste po meri občutljive informacije, uporabite naslednji članek za informacije o tem, kako ustvariti po meri občutljive vrste: [Ustvari vrsto meri občutljivih informacij](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="c9c03-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="c9c03-114">**Test DLP politike**</span><span class="sxs-lookup"><span data-stu-id="c9c03-114">**Test a DLP policy**</span></span>

<span data-ttu-id="c9c03-115">Preizkusiti svoje podatke z vrsto vgrajenih ali prilagojenih občutljive informacije, uporabite **preskus tipa** možnost iz **klasifikacije** > **vrst občutljivih informacij**.</span><span class="sxs-lookup"><span data-stu-id="c9c03-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="c9c03-116">Če želite več informacij, glejte [Test meri občutljivih podatkov vrste](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="c9c03-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="c9c03-117">**Poročila**</span><span class="sxs-lookup"><span data-stu-id="c9c03-117">**Reports**</span></span>
  
- <span data-ttu-id="c9c03-118">Dobili vpogled občutljivih podatkov s [DLP poročila.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="c9c03-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="c9c03-119">Glej podrobnosti o dogodku, [Poročilo o incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="c9c03-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
