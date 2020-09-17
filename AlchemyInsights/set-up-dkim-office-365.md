---
title: Nastavitev DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808723"
---
# <a name="setup-dkim"></a><span data-ttu-id="dabf7-102">Nastavitev DKIM</span><span class="sxs-lookup"><span data-stu-id="dabf7-102">Setup DKIM</span></span>

<span data-ttu-id="dabf7-103">Dokončana navodila za konfiguriranje DKIM za domene po meri v storitvi Microsoft 365 so [tukaj](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="dabf7-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="dabf7-104">Za **vsako** domeno po meri morate ustvariti **dva** DKIM zapisa CNAME pri ponudniku storitev gostovanja DNS domene (običajno je Registrator domene).</span><span class="sxs-lookup"><span data-stu-id="dabf7-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="dabf7-105">Na primer contoso.com in fourthcoffee.com zahtevajo štiri zapise CNAME DKIM: dva za contoso.com in dve za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="dabf7-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="dabf7-106">Zapisi CNAME DKIM za **vsako** domeno po meri uporabljajo te oblike zapisa:</span><span class="sxs-lookup"><span data-stu-id="dabf7-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="dabf7-107">**Ime gostitelja**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="dabf7-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="dabf7-108">**Pokaže na naslov ali vrednost**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="dabf7-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="dabf7-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="dabf7-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="dabf7-110">**Ime gostitelja**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="dabf7-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="dabf7-111">**Pokaže na naslov ali vrednost**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="dabf7-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="dabf7-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="dabf7-112">**TTL**: 3600</span></span>

   <span data-ttu-id="dabf7-113">\<DomainGUID\> je besedilo levo od `.mail.protection.outlook.com` zapisa prilagojene MX za domeno po meri (na primer `contoso-com` za domeno contoso.com).</span><span class="sxs-lookup"><span data-stu-id="dabf7-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="dabf7-114">\<InitialDomain\> je domena, ki ste jo uporabili, ko ste se prijavili za Microsoft 365 (na primer contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="dabf7-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="dabf7-115">Ko ustvarite zapise CNAME za domene po meri, dokončajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="dabf7-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="dabf7-116">v.</span><span class="sxs-lookup"><span data-stu-id="dabf7-116">a.</span></span> <span data-ttu-id="dabf7-117">[Vpišite se v Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) s službenim ali šolskim računom.</span><span class="sxs-lookup"><span data-stu-id="dabf7-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="dabf7-118">b.</span><span class="sxs-lookup"><span data-stu-id="dabf7-118">b.</span></span> <span data-ttu-id="dabf7-119">Izberite ikono zaganjalnika programov v zgornjem levem kotu in izberite **skrbnik**.</span><span class="sxs-lookup"><span data-stu-id="dabf7-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="dabf7-120">c.</span><span class="sxs-lookup"><span data-stu-id="dabf7-120">c.</span></span> <span data-ttu-id="dabf7-121">V spodnjem levem podoknu za krmarjenje razširite možnost **skrbnik** in izberite **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="dabf7-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="dabf7-122">d.</span><span class="sxs-lookup"><span data-stu-id="dabf7-122">d.</span></span> <span data-ttu-id="dabf7-123">Pojdite v razdelek **zaščita**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="dabf7-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="dabf7-124">e.</span><span class="sxs-lookup"><span data-stu-id="dabf7-124">e.</span></span> <span data-ttu-id="dabf7-125">Izberite domeno in nato izberite **Omogoči** za **podpisovanje sporočil za to domeno s podpisi DKIM**.</span><span class="sxs-lookup"><span data-stu-id="dabf7-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="dabf7-126">Ponovite ta korak za vsako domeno po meri.</span><span class="sxs-lookup"><span data-stu-id="dabf7-126">Repeat this step for each custom domain.</span></span>
