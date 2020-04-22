---
title: Nastavitev DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645688"
---
# <a name="setup-dkim"></a><span data-ttu-id="7a3ea-102">Nastavitev DKIM</span><span class="sxs-lookup"><span data-stu-id="7a3ea-102">Setup DKIM</span></span>

<span data-ttu-id="7a3ea-103">Popolna navodila za konfiguriranje DKIM za domene po meri v Microsoft 365 so [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="7a3ea-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="7a3ea-104">Za **vsako** domeno po meri morate ustvariti **dva** zapisa DKIM CNAME v storitvi gostovanja DNS domene (običajno registrar domene).</span><span class="sxs-lookup"><span data-stu-id="7a3ea-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="7a3ea-105">Contoso.com in fourthcoffee.com na primer zahtevata štiri zapise DKIM CNAME: dve za contoso.com in dva za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="7a3ea-106">Zapisi DKIM CNAME za **vsako** domeno po meri uporabljajo naslednje formate:</span><span class="sxs-lookup"><span data-stu-id="7a3ea-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="7a3ea-107">**Ime gostitelja**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="7a3ea-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="7a3ea-108">**Točke za naslov ali vrednost**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="7a3ea-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="7a3ea-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="7a3ea-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="7a3ea-110">**Ime gostitelja**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="7a3ea-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="7a3ea-111">**Točke za naslov ali vrednost**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="7a3ea-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="7a3ea-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="7a3ea-112">**TTL**: 3600</span></span>

   <span data-ttu-id="7a3ea-113">\<DomainGUID\> je besedilo v levem `.mail.protection.outlook.com` zapisu po meri MX za domeno po meri (na primer `contoso-com` za domeno contoso.com).</span><span class="sxs-lookup"><span data-stu-id="7a3ea-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="7a3ea-114">\<InitialDomain\> je domena, ki ste jo uporabili, ko ste se prijavili za Microsoft 365 (na primer contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="7a3ea-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="7a3ea-115">Ko ustvarite zapise CNAME za domene po meri, izpolnite ta navodila:</span><span class="sxs-lookup"><span data-stu-id="7a3ea-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="7a3ea-116">A.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-116">a.</span></span> <span data-ttu-id="7a3ea-117">[Vpišite se v Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s svojim delovnim ali šolskim računom.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="7a3ea-118">B.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-118">b.</span></span> <span data-ttu-id="7a3ea-119">V zgornjem levem kotu izberite ikono zaganjalnika aplikacij in izberite **skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="7a3ea-120">C.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-120">c.</span></span> <span data-ttu-id="7a3ea-121">V spodnjem levem krmarjenju razširite možnost **skrbnik** in izberite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="7a3ea-122">D.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-122">d.</span></span> <span data-ttu-id="7a3ea-123">Pojdi na **zaščito** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="7a3ea-124">E.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-124">e.</span></span> <span data-ttu-id="7a3ea-125">Izberite domeno in nato izberite **Omogoči** za **podpisovanje sporočil za to DOMENO s podpisi DKIM**.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="7a3ea-126">Ponovite ta korak za vsako domeno po meri.</span><span class="sxs-lookup"><span data-stu-id="7a3ea-126">Repeat this step for each custom domain.</span></span>
