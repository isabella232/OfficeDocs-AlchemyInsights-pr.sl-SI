---
title: Težave pri razvoju programov z API-ji
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975018"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="f30d5-102">Težave pri razvoju programov z API-ji</span><span class="sxs-lookup"><span data-stu-id="f30d5-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="f30d5-103">Za začetek uporabe API-ja v storitvi Azure Active Directory je na [sporedu vodnik AZURE ad GRAPH API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , ali pa si oglejte dokumentacijo priročnika [interaktivnih](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)grafičnih grafikonov Azure ad.</span><span class="sxs-lookup"><span data-stu-id="f30d5-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="f30d5-104">**Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL) in Azure AD Graph API (graf ZVOČNIh grafikonov)**</span><span class="sxs-lookup"><span data-stu-id="f30d5-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="f30d5-105">Z **začetkom junija 30th 2020** ne bomo več dodali nobenih novih funkcij v knjižnice adal in Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="f30d5-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="f30d5-106">Še naprej bomo zagotavljali tehnično podporo in varnostne posodobitve, vendar ne boste mogli več posredovati posodobitev funkcij.</span><span class="sxs-lookup"><span data-stu-id="f30d5-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="f30d5-107">Z **začetkom junija 30th 2022** bomo zaključili podporo za knjižnice adal in Azure ad Graph in ne boste več zagotavljali tehnične podpore ali varnostnih posodobitev.</span><span class="sxs-lookup"><span data-stu-id="f30d5-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="f30d5-108">Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo prejeli nobene tehnične podpore ali varnostnih posodobitev.</span><span class="sxs-lookup"><span data-stu-id="f30d5-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="f30d5-109">Programi, ki uporabljajo Azure AD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne točke grafikona Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f30d5-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="f30d5-110">**Selitev v knjižnice ADAL**</span><span class="sxs-lookup"><span data-stu-id="f30d5-110">**ADAL Migration**</span></span>

<span data-ttu-id="f30d5-111">Priporočamo, da posodobite [Microsoftovo knjižnico za preverjanje pristnosti (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), ki ima najnovejše funkcije in varnostne posodobitve.</span><span class="sxs-lookup"><span data-stu-id="f30d5-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="f30d5-112">Če uporabljate Microsoft apps, veste, da je Microsoft v postopku selitve svojih programov v MSAL z rokom za konec podpore, s čimer zagotovite, da bodo imeli koristi od trenutne varnosti in izboljšav funkcij v MSAL.</span><span class="sxs-lookup"><span data-stu-id="f30d5-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="f30d5-113">[Preberite pogosta vprašanja o knjižnice adal](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="f30d5-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="f30d5-114">[Preberite več o tem, kako preseliti aplikacije na osnovi na platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="f30d5-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="f30d5-115">Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, vam priporočamo, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne ISVs ali ponudnike programov.</span><span class="sxs-lookup"><span data-stu-id="f30d5-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="f30d5-116">Microsoftova podpora vam omogoča tudi seznam vseh programov, ki niso Microsoftovi za knjižnice ADAL, v najemniku.</span><span class="sxs-lookup"><span data-stu-id="f30d5-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="f30d5-117">**Selitev diagrama ZVOČNIh grafikonov**</span><span class="sxs-lookup"><span data-stu-id="f30d5-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="f30d5-118">Za programe, ki uporabljajo grafiko Azure AD Graph, upoštevajte navodila za selitev [programov AZURE ad Graph v Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="f30d5-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="f30d5-119">[Naš kontrolni seznam selitve zagotavlja uvodno mesto](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="f30d5-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="f30d5-120">V portalu za registracijo aplikacije Azure so prikazani programi, ki uporabljajo ZVOČNI diagram.</span><span class="sxs-lookup"><span data-stu-id="f30d5-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="f30d5-121">Priporočamo vam, da pregledate vse izvorne kode programov in po potrebi poiščete vse ponudnike ISVs ali aplikacije.</span><span class="sxs-lookup"><span data-stu-id="f30d5-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="f30d5-122">Microsoftova podpora vam omogoča tudi seznam vseh uporab ZVOČNIh grafikonov v najemniku.</span><span class="sxs-lookup"><span data-stu-id="f30d5-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="f30d5-123">Če želite za program dostopati do podatkov v programu Microsoft Graph, ga mora uporabnik ali skrbnik dodeliti pravilnim dovoljenjem prek postopka soglasja.</span><span class="sxs-lookup"><span data-stu-id="f30d5-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="f30d5-124">[Sklici na dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) navajajo dovoljenja, povezana z vsakim glavnim naborom API-jev Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f30d5-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="f30d5-125">Na voljo so tudi navodila za uporabo dovoljenj.</span><span class="sxs-lookup"><span data-stu-id="f30d5-125">It also provides guidance about how to use the permissions.</span></span>
