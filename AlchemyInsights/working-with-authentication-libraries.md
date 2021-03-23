---
title: Delo s knjižnicami za preverjanje pristnosti
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036868"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="98d4e-102">Delo s knjižnicami za preverjanje pristnosti</span><span class="sxs-lookup"><span data-stu-id="98d4e-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="98d4e-103">Če želite odpraviti težavo z Microsoftovo knjižnico za preverjanje pristnosti (MSAL), izvedite te priporočene korake:</span><span class="sxs-lookup"><span data-stu-id="98d4e-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="98d4e-104">**Delo z MSAL**: [knjižnice za preverjanje pristnosti za Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – v tem članku je prikazana podpora knjižnice za Microsoft preverjanje pristnosti za več vrst aplikacij.</span><span class="sxs-lookup"><span data-stu-id="98d4e-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="98d4e-105">Vključuje povezave do izvorne kode knjižnice; kje dobiti paket za projekt programa; in ali knjižnica podpira vpis uporabnika (preverjanje pristnosti), dostop do zaščitenih spletnih vmesnikov API (avtorizacija) ali oboje.</span><span class="sxs-lookup"><span data-stu-id="98d4e-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="98d4e-106">**Odpravljanje težav s preverjanjem pristnosti**: MSAL podpira več tokov preverjanja pristnosti za uporabo v različnih scenarijih programov.</span><span class="sxs-lookup"><span data-stu-id="98d4e-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="98d4e-107">Odvisno od tega, kako je vaš odjemalski program zgrajen, lahko MSAL uporabi enega ali več tokov preverjanja pristnosti, ki jih podpira Microsoftova platforma Identity.</span><span class="sxs-lookup"><span data-stu-id="98d4e-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="98d4e-108">Ti tokovi lahko ustvarijo več vrst žetonov in šifer dovoljenj ter zahtevajo različne žetone, da bodo delovali.</span><span class="sxs-lookup"><span data-stu-id="98d4e-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="98d4e-109">**Žetoni za dostop**: [žetoni za dostop do Microsoftovega](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) uporabniškega vmesnika – Preberite, kako lahko API preveri veljavnost in uporabi terjatve znotraj žetona za dostop.</span><span class="sxs-lookup"><span data-stu-id="98d4e-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="98d4e-110">Vsa dokumentacija v tem članku, razen če je označeno, velja le za žetone, izdane za API-je, ki ste jih registrirali.</span><span class="sxs-lookup"><span data-stu-id="98d4e-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="98d4e-111">Ne velja za žetone, izdane za Microsoft lastne API-je, ne morete pa uporabiti teh žetonov za preverjanje, kako Microsoftova identitetna platforma izdaja žetone za API, ki jih ustvarite.</span><span class="sxs-lookup"><span data-stu-id="98d4e-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="98d4e-112">**Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL)**</span><span class="sxs-lookup"><span data-stu-id="98d4e-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="98d4e-113">Z **začetkom junija 30th 2020** ne bomo več dodali nobenih novih funkcij v knjižnice adal in Azure ad Graph.</span><span class="sxs-lookup"><span data-stu-id="98d4e-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="98d4e-114">Še naprej nudimo tehnično podporo in varnostne posodobitve, ne zagotavljamo pa več posodobitev funkcij.</span><span class="sxs-lookup"><span data-stu-id="98d4e-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="98d4e-115">Z **začetkom junija 30th 2022** bomo zaključili podporo za knjižnice adal in Azure ad Graph in ne boste več zagotavljali tehnične podpore ali varnostnih posodobitev.</span><span class="sxs-lookup"><span data-stu-id="98d4e-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="98d4e-116">Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo *prejeli nobene tehnične podpore ali varnostnih posodobitev*.</span><span class="sxs-lookup"><span data-stu-id="98d4e-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="98d4e-117">Programi, ki uporabljajo Azure AD Graph, po tem času morda ne bodo več prejemali odgovorov iz končne točke grafikona Azure AD.</span><span class="sxs-lookup"><span data-stu-id="98d4e-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="98d4e-118">**Selitev v knjižnice ADAL**</span><span class="sxs-lookup"><span data-stu-id="98d4e-118">**ADAL Migration**</span></span>

- <span data-ttu-id="98d4e-119">Priporočamo, da posodobite MSAL, ki vsebuje najnovejše funkcije in varnostne posodobitve.</span><span class="sxs-lookup"><span data-stu-id="98d4e-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="98d4e-120">Če uporabljate Microsoft apps, morate vedeti, da je Microsoft v postopku selitve svojih programov v MSAL s končnim rokom za konec podpore, ki zagotavlja, da bodo imeli koristi od trenutne varnosti in izboljšav funkcij v MSAL.</span><span class="sxs-lookup"><span data-stu-id="98d4e-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="98d4e-121">[Preberite pogosta vprašanja o knjižnice adal](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="98d4e-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="98d4e-122">[Preberite več o tem, kako preseliti aplikacije na osnovi na platformi](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="98d4e-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="98d4e-123">Če imate po branju priročnika za platformo aplikacije na voljo dodatna vprašanja, lahko objavite na [spletnem mestu Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) z oznako [Azure-ad-knjižnice adal-zastaranje] ali pa odprete težavo v skladišču mesta GitHub v knjižnici.</span><span class="sxs-lookup"><span data-stu-id="98d4e-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="98d4e-124">Oglejte si razdelek [jeziki in okviri](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) v članku **MSAL pregled** članka za povezave do repo posameznih knjižnic.</span><span class="sxs-lookup"><span data-stu-id="98d4e-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="98d4e-125">**Če potrebujete pomoč pri razumevanju, kateri programi uporabljajo knjižnice adal**, priporočamo, da pregledate vse izvorne kode aplikacije.</span><span class="sxs-lookup"><span data-stu-id="98d4e-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="98d4e-126">Po potrebi se povežite s katerim koli neodvisnim prodajalcem programske opreme (ISVs) ali ponudnikom aplikacij.</span><span class="sxs-lookup"><span data-stu-id="98d4e-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="98d4e-127">Microsoftova podpora vam lahko posreduje seznam vseh aplikacij ADAL v vašem najemniku, ki jih ne zagotavlja Microsoft.</span><span class="sxs-lookup"><span data-stu-id="98d4e-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







