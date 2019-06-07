---
title: Nastavitev DKIM v Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765429"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="eb250-102">Nastavitev DKIM v Office 365</span><span class="sxs-lookup"><span data-stu-id="eb250-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="eb250-103">Celotna navodila za konfiguracijo DKIM za custom domene v Office 365 so [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="eb250-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="eb250-104">Za **vsako** domeno, po meri, morate ustvariti **dva** DKIM CNAME zapisi na vaše domene DNS gostovanje storitev (praviloma registratorja domene).</span><span class="sxs-lookup"><span data-stu-id="eb250-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="eb250-105">Na primer contoso.com in fourthcoffee.com zahtevajo štiri zapise DKIM CNAME: dve za contoso.com in dva za fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="eb250-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="eb250-106">DKIM CNAME zapisov za **vsako** domeno po meri uporabite naslednje formate:</span><span class="sxs-lookup"><span data-stu-id="eb250-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="eb250-107">**Ime gostitelja**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="eb250-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="eb250-108">**Točki naslov ali vrednost**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="eb250-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="eb250-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="eb250-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="eb250-110">**Ime gostitelja**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="eb250-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="eb250-111">**Točki naslov ali vrednost**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="eb250-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="eb250-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="eb250-112">**TTL**: 3600</span></span>

   <span data-ttu-id="eb250-113">\<DomainGUID\> je besedilo levo od `.mail.protection.outlook.com` v prilagojeno zapis MX za domeno po meri (na primer, `contoso-com` za domeno contoso.com).</span><span class="sxs-lookup"><span data-stu-id="eb250-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="eb250-114">\<InitialDomain\> je domena, ki ste ga uporabili, ko ste se prijavili za program Office 365 (na primer, contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="eb250-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="eb250-115">Ko ustvarite zapise CNAME za custom domene, izpolnite naslednja navodila:</span><span class="sxs-lookup"><span data-stu-id="eb250-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="eb250-116">a.</span><span class="sxs-lookup"><span data-stu-id="eb250-116">a.</span></span> <span data-ttu-id="eb250-117">[Prijavite se v Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) z računom delo ali v šolo.</span><span class="sxs-lookup"><span data-stu-id="eb250-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="eb250-118">b.</span><span class="sxs-lookup"><span data-stu-id="eb250-118">b.</span></span> <span data-ttu-id="eb250-119">Izberite ikono app pobudnik v zgornjem desnem in izberite **Admin**.</span><span class="sxs-lookup"><span data-stu-id="eb250-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="eb250-120">c.</span><span class="sxs-lookup"><span data-stu-id="eb250-120">c.</span></span> <span data-ttu-id="eb250-121">V spodnjem levem navigacija, razširite **Admin** in izberite **izmenjavo**.</span><span class="sxs-lookup"><span data-stu-id="eb250-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="eb250-122">d.</span><span class="sxs-lookup"><span data-stu-id="eb250-122">d.</span></span> <span data-ttu-id="eb250-123">Pojdi na **varstvo** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="eb250-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="eb250-124">e.</span><span class="sxs-lookup"><span data-stu-id="eb250-124">e.</span></span> <span data-ttu-id="eb250-125">Izberite domeno in izberite **Omogoči** za **znak sporočila za to domeno z DKIM podpisov**.</span><span class="sxs-lookup"><span data-stu-id="eb250-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="eb250-126">Ponovite ta korak za vsako domeno po meri.</span><span class="sxs-lookup"><span data-stu-id="eb250-126">Repeat this step for each custom domain.</span></span>
