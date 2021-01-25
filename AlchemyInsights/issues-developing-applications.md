---
title: Težave z razvojem programov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974767"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="0dbcb-102">Težave z razvojem programov</span><span class="sxs-lookup"><span data-stu-id="0dbcb-102">Issues developing applications</span></span>

<span data-ttu-id="0dbcb-103">Če želite odpraviti najpogostejše težave pri gradnji programov Azure Active Directory (AD), si oglejte te članke:</span><span class="sxs-lookup"><span data-stu-id="0dbcb-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="0dbcb-104">Vidim težave pri vpisu v program le z brskalnikom Chrome</span><span class="sxs-lookup"><span data-stu-id="0dbcb-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="0dbcb-105">Ne vem, kako naj spremenim privzete nastavitve žetona za moj program</span><span class="sxs-lookup"><span data-stu-id="0dbcb-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="0dbcb-106">Sem zbegan o tem, kako deluje soglasje aplikacije</span><span class="sxs-lookup"><span data-stu-id="0dbcb-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="0dbcb-107">Ne vem, kako dodeliti dovoljenja za moj program</span><span class="sxs-lookup"><span data-stu-id="0dbcb-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="0dbcb-108">Ne razumem razlike med delegiranimi in dovoljenji za uporabo</span><span class="sxs-lookup"><span data-stu-id="0dbcb-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="0dbcb-109">\***Konec podpore za knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice adal) in AZURE ad GRAPH API (zvočni grafikon)** _</span><span class="sxs-lookup"><span data-stu-id="0dbcb-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="0dbcb-110">Z začetkom junija 30th 2020 ne bomo več dodali nobenih novih funkcij v knjižnico za preverjanje pristnosti v storitvi Azure Active Directory (knjižnice ADAL) in Azure AD Graph API (ZVOČNI grafikon).</span><span class="sxs-lookup"><span data-stu-id="0dbcb-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="0dbcb-111">Še naprej bomo zagotavljali tehnično podporo in varnostne posodobitve, vendar ne boste mogli več posredovati posodobitev funkcij.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="0dbcb-112">Z začetkom junija 30th 2022 bomo zaključili podporo za knjižnice ADAL in ZVOČNI diagram ter ne bodo več zagotavljali tehnične podpore ali varnostnih posodobitev.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="0dbcb-113">Zaradi tega pogoja so te posledice:</span><span class="sxs-lookup"><span data-stu-id="0dbcb-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="0dbcb-114">Programi, ki uporabljajo knjižnice ADAL v obstoječih različicah sistema OS, bodo po tem času še naprej delovali, vendar ne bodo prejeli nobene tehnične podpore ali varnostnih posodobitev.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="0dbcb-115">Programi, ki uporabljajo ZVOČNI diagram, po tem času morda ne bodo več prejemali odgovorov iz končne točke v grafu ZVOČNIka</span><span class="sxs-lookup"><span data-stu-id="0dbcb-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="0dbcb-116">_ *Knjižnice adal selitev*\*</span><span class="sxs-lookup"><span data-stu-id="0dbcb-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="0dbcb-117">Če uporabljate Microsoft apps, priporočamo, da posodobite Microsoftovo knjižnico za preverjanje pristnosti (MSAL), ki ima najnovejše funkcije in varnostne posodobitve.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="0dbcb-118">To priporočilo je v kontekstu Microsoft, ki uvaja postopek selitve svojih programov v MSAL z rokom konca podpore.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="0dbcb-119">Selitev Microsoft svojih aplikacij v MSAL zagotavlja, da bodo aplikacije izkoristile prednosti sprotne varnosti in izboljšav funkcij MSAL.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="0dbcb-120">Preberite pogosta vprašanja o knjižnice ADAL</span><span class="sxs-lookup"><span data-stu-id="0dbcb-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="0dbcb-121">Preberite več o tem, kako preseliti aplikacije na osnovi na platformi</span><span class="sxs-lookup"><span data-stu-id="0dbcb-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="0dbcb-122">Če potrebujete pomoč pri razumevanju, katere aplikacije uporabljajo knjižnice ADAL, priporočamo, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne neodvisne prodajalce programske opreme (ISVs) ali ponudnike programov.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="0dbcb-123">Microsoftova podpora vam omogoča tudi seznam vseh programov, ki niso Microsoftovi za knjižnice ADAL, v najemniku.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="0dbcb-124">**Selitev diagrama ZVOČNIh grafikonov**</span><span class="sxs-lookup"><span data-stu-id="0dbcb-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="0dbcb-125">Za programe, ki uporabljajo ZVOČNI graf, upoštevajte naše napotke za selitev programov ZVOČNIh grafikonov v Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="0dbcb-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="0dbcb-126">[Naš kontrolni seznam selitve zagotavlja uvodno mesto](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="0dbcb-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="0dbcb-127">V portalu za registracijo aplikacije Azure so prikazani programi, ki uporabljajo ZVOČNI diagram.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="0dbcb-128">Priporočamo vam, da pregledate vse izvorne kode programov in po potrebi poiščete morebitne neodvisne prodajalce programske opreme (ISVs) ali ponudnike programov.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="0dbcb-129">Microsoftova podpora vam omogoča tudi informacije o uporabi ZVOČNIh grafikonov v najemniku.</span><span class="sxs-lookup"><span data-stu-id="0dbcb-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







