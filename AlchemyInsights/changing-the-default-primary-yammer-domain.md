---
title: Spreminjanje privzete domene Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 6a7215ef7187e8dc6c834470b4724692b239efd4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818016"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a><span data-ttu-id="dd189-102">Spreminjanje privzete/primarne domene Yammer</span><span class="sxs-lookup"><span data-stu-id="dd189-102">Changing the default/primary Yammer domain</span></span>

<span data-ttu-id="dd189-103">URL Yammer vsebuje trenutno primarno ime domene za vaše omrežje Yammer.</span><span class="sxs-lookup"><span data-stu-id="dd189-103">The Yammer URL contains the current primary domain name for your Yammer network.</span></span> <span data-ttu-id="dd189-104">To ime domene se morda ne bo ujemalo z imenom primarne domene v sistemu Office 365 ali Azure AD.</span><span class="sxs-lookup"><span data-stu-id="dd189-104">This domain name may not match the primary domain name set in Office 365 or Azure AD.</span></span> <span data-ttu-id="dd189-105">Glede na število domen po meri, ki so bile dodane najemniku, obstajajo razlike, in ali je Yammer podprta konfiguracija (1 najemnik: 1 omrežje ali 1:1).</span><span class="sxs-lookup"><span data-stu-id="dd189-105">There are differences in behavior based on the number of custom domains added to the tenant, and whether Yammer is in a supported configuration (1 Tenant: 1 Network, or 1:1).</span></span> <span data-ttu-id="dd189-106">Dokumentacija o [Yammer domenah in Officeu 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) je na voljo.</span><span class="sxs-lookup"><span data-stu-id="dd189-106">Documentation on [Yammer domains and Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) is available.</span></span>

<span data-ttu-id="dd189-107">Najpogostejši razlog, zaradi katerega je nepravilna domena, je, da obstaja več Yammer omrežij in jih je treba združiti.</span><span class="sxs-lookup"><span data-stu-id="dd189-107">The most common reason that you see an incorrect domain is that multiple Yammer networks exist and need to be consolidated.</span></span> <span data-ttu-id="dd189-108">[Z orodjem za selitev omrežja lahko združite v eno samo omrežje](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) je pomemben prvi korak.</span><span class="sxs-lookup"><span data-stu-id="dd189-108">[Consolidating down to a single network](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) using the network migration tool is an important first step.</span></span> <span data-ttu-id="dd189-109">Preden začnete nastavljati primarno domeno, dokončajte ta postopek.</span><span class="sxs-lookup"><span data-stu-id="dd189-109">Complete this before attempting to set your primary domain.</span></span>

<span data-ttu-id="dd189-110">**Brez domen po meri**</span><span class="sxs-lookup"><span data-stu-id="dd189-110">**No custom domains**</span></span>

<span data-ttu-id="dd189-111">Za nove najemnike bo privzeta domena (na primer fabrikam.onmicrosoft.com) iz najemnika uporabljena za Yammer.</span><span class="sxs-lookup"><span data-stu-id="dd189-111">For new tenants, the default domain (e.g. fabrikam.onmicrosoft.com) from the tenant will be used for Yammer.</span></span> <span data-ttu-id="dd189-112">Primarna domena je nastavljena na yammer.com/fabrikam.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="dd189-112">The primary domain is set to yammer.com/fabrikam.onmicrosoft.com.</span></span>

<span data-ttu-id="dd189-113">**Ena domena po meri**</span><span class="sxs-lookup"><span data-stu-id="dd189-113">**Single custom domain**</span></span>

<span data-ttu-id="dd189-114">Yammer bo samodejno izbral domeno po meri (npr. fabrikam.com) iz najemnika kot primarno domeno v Yammer.</span><span class="sxs-lookup"><span data-stu-id="dd189-114">Yammer will automatically select the custom domain (e.g. fabrikam.com) from the tenant as the primary domain in Yammer.</span></span> <span data-ttu-id="dd189-115">Nastavljena je na yammer.com/fabrikam.com.</span><span class="sxs-lookup"><span data-stu-id="dd189-115">It is set to yammer.com/fabrikam.com.</span></span> <span data-ttu-id="dd189-116">Ta sprememba je izvedena s storitvijo za sinhronizacijo domen in lahko začne veljati do 24 ur.</span><span class="sxs-lookup"><span data-stu-id="dd189-116">This change is made by the domain sync service, and can take up to 24 hours to take effect.</span></span>

<span data-ttu-id="dd189-117">**Številne domene po meri**</span><span class="sxs-lookup"><span data-stu-id="dd189-117">**Multiple custom domains**</span></span>

<span data-ttu-id="dd189-118">Yammer ima lahko primarno domeno, ki se razlikuje od privzete domene najemnika.</span><span class="sxs-lookup"><span data-stu-id="dd189-118">Yammer can have a primary domain that is different from the default tenant domain.</span></span> <span data-ttu-id="dd189-119">Ker je na voljo več domen po meri, Yammer ne poskuša ugibati pravilne domene od razpoložljivih.</span><span class="sxs-lookup"><span data-stu-id="dd189-119">Since there are multiple custom domains, Yammer does not attempt to guess the correct domain from those available.</span></span> <span data-ttu-id="dd189-120">Če želite zahtevati, da je primarno ime domene spremenjeno na primarno domeno, ki jo želite izbrati, morate odpreti primer podpore.</span><span class="sxs-lookup"><span data-stu-id="dd189-120">You need to open a support case to request that the primary domain name is changed to the primary domain of your choice.</span></span>

<span data-ttu-id="dd189-121">**Dodatne informacije za odpravljanje težav**</span><span class="sxs-lookup"><span data-stu-id="dd189-121">**Additional troubleshooting information**</span></span>

<span data-ttu-id="dd189-122">V nekaterih primerih se je morda premaknilo med najemniki in storitev za sinhronizacijo domen se ni uspešno zagnala.</span><span class="sxs-lookup"><span data-stu-id="dd189-122">In some cases domains may have been moved between tenants and the domain sync service has not been able to run successfully.</span></span> <span data-ttu-id="dd189-123">Poleg nepravilne primarne domene lahko pride tudi do vpisa ali drugih težav.</span><span class="sxs-lookup"><span data-stu-id="dd189-123">You may experience sign-in or other issues, in addition to an incorrect primary domain.</span></span> <span data-ttu-id="dd189-124">Če želite odpraviti to težavo, boste morda morali domene prestaviti v pravo omrežje s pomočjo Microsoftove podpore.</span><span class="sxs-lookup"><span data-stu-id="dd189-124">To resolve this problem, domains may need to be moved to the correct network with help from Microsoft Support.</span></span> <span data-ttu-id="dd189-125">Ta situacija zahteva neposredno pomoč in lahko traja nekaj časa, še posebej, če je na voljo zelo dolg seznam domenskih imen.</span><span class="sxs-lookup"><span data-stu-id="dd189-125">This situation requires direct assistance and can take some time to resolve, especially if there is a very long list of domain names.</span></span> <span data-ttu-id="dd189-126">Odpiranje primera podpore za pomoč pri odpravljanju teh vrst težav.</span><span class="sxs-lookup"><span data-stu-id="dd189-126">Open a support case to get assistance with resolving these types of issues.</span></span>

<span data-ttu-id="dd189-127">Ko delate s posrednikom za podporo, bodo preverili, ali so domene preverjene v najemniku pod vašim nadzorom.</span><span class="sxs-lookup"><span data-stu-id="dd189-127">When working with a support agent, they will check that domains are verified on a tenant under your control.</span></span> <span data-ttu-id="dd189-128">Če so dodane v vašega najemnika, ne da bi jih preverili zapisi DNS, lahko zahtevajo dodatna vprašanja za preverjanje glede domen.</span><span class="sxs-lookup"><span data-stu-id="dd189-128">They may ask additional verification questions about your domains if they are added to your tenant but not verified by DNS.</span></span> <span data-ttu-id="dd189-129">Prepričajte se, da je DNS preverjanje domen preverjeno tako, da pospeši postopek.</span><span class="sxs-lookup"><span data-stu-id="dd189-129">Please ensure that domains are verified by DNS to speed up the process.</span></span>
