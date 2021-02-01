---
title: Težave s knjižnicami za preverjanje pristnosti
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063645"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="d4c6c-102">Težave s knjižnicami za preverjanje pristnosti</span><span class="sxs-lookup"><span data-stu-id="d4c6c-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="d4c6c-103">[Knjižnice za preverjanje pristnosti za Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) je na voljo za Microsoftove podprte in nezdružljive knjižnice odjemalca in vmesnega seznama.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="d4c6c-104">Microsoftova knjižnica za preverjanje pristnosti (MSAL) podpira več [tokov preverjanja pristnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) za uporabo v različnih scenarijih programov.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="d4c6c-105">Če želite preveriti pristnost in pridobiti žetone, inicializirate nov javni ali zaupen odjemalski program v kodi.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="d4c6c-106">Ko inicializirate odjemalski program v Microsoftovi knjižnici za preverjanje pristnosti (MSAL), lahko nastavite več možnosti konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="d4c6c-107">Če želite izvedeti več, glejte [možnosti konfiguracije aplikacije](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="d4c6c-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="d4c6c-108">**Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL) in Azure AD Graph API (graf ZVOČNIh grafikonov)**</span><span class="sxs-lookup"><span data-stu-id="d4c6c-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="d4c6c-109">Z **začetkom junija 30th 2020** ne bomo več dodali nobenih novih funkcij v knjižnice adal in Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="d4c6c-110">Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="d4c6c-111">Z **začetkom junija 30th 2022** bomo zaključili podporo za knjižnice adal in Azure ad Graph in ne boste več zagotavljali tehnične podpore ali varnostnih posodobitev.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="d4c6c-112">Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo *prejeli nobene tehnične podpore ali varnostnih posodobitev*.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="d4c6c-113">Programi, ki uporabljajo Azure AD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne točke grafikona Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="d4c6c-114">**Selitev v knjižnice ADAL**</span><span class="sxs-lookup"><span data-stu-id="d4c6c-114">**ADAL Migration**</span></span>

<span data-ttu-id="d4c6c-115">Priporočamo, da izvedete nadgradnjo na knjižnico [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki vključuje najnovejše funkcije in varnostne posodobitve.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="d4c6c-116">Če uporabljate Microsoft apps, veste, da je Microsoft v postopku selitve svojih programov v MSAL z rokom za konec podpore, s čimer zagotovi, da bodo imeli koristi od trenutne varnosti in izboljšav funkcij v MSAL.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="d4c6c-117">Za več informacij glejte:</span><span class="sxs-lookup"><span data-stu-id="d4c6c-117">For more information, see:</span></span>

1. [<span data-ttu-id="d4c6c-118">Preberite pogosta vprašanja o knjižnici ADAL</span><span class="sxs-lookup"><span data-stu-id="d4c6c-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="d4c6c-119">Več informacij o selitvi aplikacij glede na platformo</span><span class="sxs-lookup"><span data-stu-id="d4c6c-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="d4c6c-120">Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, vam priporočamo, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne ISVs ali ponudnike programov.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="d4c6c-121">Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="d4c6c-122">**Selitev zmogljivosti AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="d4c6c-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="d4c6c-123">Za programe, ki uporabljajo grafiko Azure AD Graph, upoštevajte navodila za [selitev programov AZURE ad Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="d4c6c-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="d4c6c-124">Naš kontrolni seznam selitve zagotavlja uvodno mesto.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="d4c6c-125">Na portalu za registracijo aplikacije Azure so prikazane aplikacije, ki uporabljajo AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="d4c6c-126">Priporočamo, da pregledate izvorno kodo vseh aplikacij ter po potrebi stopite v stik z morebitnimi neodvisnimi razvijalci programske opreme ali ponudniki aplikacij.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="d4c6c-127">Microsoftova podpora vam omogoča tudi seznam vseh uporab ZVOČNIh grafikonov v najemniku.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="d4c6c-128">Če želite za program dostopati do podatkov v programu Microsoft Graph, ga mora uporabnik ali skrbnik dodeliti pravilnim dovoljenjem prek postopka soglasja.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="d4c6c-129">[Sklici na dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) navajajo dovoljenja, povezana z vsakim glavnim naborom API-jev Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="d4c6c-130">Na voljo so tudi navodila za uporabo dovoljenj.</span><span class="sxs-lookup"><span data-stu-id="d4c6c-130">It also provides guidance about how to use the permissions.</span></span>
