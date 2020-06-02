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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509400"
---
# <a name="setup-dkim"></a><span data-ttu-id="3441f-102">Nastavitev DKIM</span><span class="sxs-lookup"><span data-stu-id="3441f-102">Setup DKIM</span></span>

<span data-ttu-id="3441f-103">Popolna navodila za konfiguriranje DKIM za domene po meri v Microsoft 365 so [tukaj](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="3441f-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="3441f-104">Za **vsako** domeno po meri morate ustvariti **dva** zapisa DKIM CNAME v storitvi gostovanja DNS domene (običajno registrar domene).</span><span class="sxs-lookup"><span data-stu-id="3441f-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="3441f-105">Contoso.com in fourthcoffee.com na primer zahtevata štiri zapise DKIM CNAME: dve za contoso.com in dva za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="3441f-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="3441f-106">Zapisi DKIM CNAME za **vsako** domeno po meri uporabljajo naslednje formate:</span><span class="sxs-lookup"><span data-stu-id="3441f-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="3441f-107">**Ime gostitelja**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="3441f-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="3441f-108">**Točke za naslov ali vrednost**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="3441f-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="3441f-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="3441f-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="3441f-110">**Ime gostitelja**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="3441f-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="3441f-111">**Točke za naslov ali vrednost**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="3441f-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="3441f-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="3441f-112">**TTL**: 3600</span></span>

   <span data-ttu-id="3441f-113">\<DomainGUID\>je besedilo na levi strani v meri `.mail.protection.outlook.com` zapisa MX za domeno po meri (na primer `contoso-com` za domeno contoso.com).</span><span class="sxs-lookup"><span data-stu-id="3441f-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="3441f-114">\<InitialDomain\>je domena, ki ste jo uporabili, ko ste se prijavili za Microsoft 365 (na primer contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="3441f-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="3441f-115">Ko ustvarite zapise CNAME za domene po meri, izpolnite ta navodila:</span><span class="sxs-lookup"><span data-stu-id="3441f-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="3441f-116">A.</span><span class="sxs-lookup"><span data-stu-id="3441f-116">a.</span></span> <span data-ttu-id="3441f-117">[Vpišite se v Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s svojim delovnim ali šolskim računom.</span><span class="sxs-lookup"><span data-stu-id="3441f-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="3441f-118">B.</span><span class="sxs-lookup"><span data-stu-id="3441f-118">b.</span></span> <span data-ttu-id="3441f-119">V zgornjem levem kotu izberite ikono zaganjalnika aplikacij in izberite **skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="3441f-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="3441f-120">C.</span><span class="sxs-lookup"><span data-stu-id="3441f-120">c.</span></span> <span data-ttu-id="3441f-121">V spodnjem levem krmarjenju razširite možnost **skrbnik** in izberite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="3441f-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="3441f-122">D.</span><span class="sxs-lookup"><span data-stu-id="3441f-122">d.</span></span> <span data-ttu-id="3441f-123">Pojdi na **zaščito**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="3441f-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="3441f-124">E.</span><span class="sxs-lookup"><span data-stu-id="3441f-124">e.</span></span> <span data-ttu-id="3441f-125">Izberite domeno in nato izberite **Omogoči** za **podpisovanje sporočil za to DOMENO s podpisi DKIM**.</span><span class="sxs-lookup"><span data-stu-id="3441f-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="3441f-126">Ponovite ta korak za vsako domeno po meri.</span><span class="sxs-lookup"><span data-stu-id="3441f-126">Repeat this step for each custom domain.</span></span>
