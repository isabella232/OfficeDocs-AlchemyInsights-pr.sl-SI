---
title: Poizvedovanje po API-ju Microsoft Graph
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974686"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="3453f-102">Poizvedovanje po API-ju Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="3453f-103">Ta tema se lahko uporablja tudi za razvijalce, ki še vedno uporabljajo vmesnik Azure AD Graph API.</span><span class="sxs-lookup"><span data-stu-id="3453f-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="3453f-104">Vendar pa **je priporočljivo,** da uporabite Microsoft Graph za vse scenarije imenika, identitete in upravljanja Accessa.</span><span class="sxs-lookup"><span data-stu-id="3453f-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="3453f-105">**Težave s preverjanjem pristnosti ali avtorizacije**</span><span class="sxs-lookup"><span data-stu-id="3453f-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="3453f-106">Če vaš program **ne more pridobiti žetonov** za klicanje programa Microsoft Graph, izberite **težave z iskanjem žetona Microsoft Graph (preverjanje pristnosti)** , da pridobite natančnejšo pomoč in podporo v tej temi.</span><span class="sxs-lookup"><span data-stu-id="3453f-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="3453f-107">Če vaš program **prejema napake pri avtorizaciji v storitvi 401 ali 403** , ko kličete Microsoft Graph, izberite kategorijo» **pridobivanje zavrnjenega dostopa «(avtorizacija)** , ki je v kategoriji API za Microsoft Graph, da pridobite natančnejšo pomoč in podporo v tej temi.</span><span class="sxs-lookup"><span data-stu-id="3453f-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="3453f-108">**Želim uporabljati Microsoft Graph, vendar ne vem, kje naj začnem**</span><span class="sxs-lookup"><span data-stu-id="3453f-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="3453f-109">Če želite izvedeti več o programu Microsoft Graph, glejte:</span><span class="sxs-lookup"><span data-stu-id="3453f-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="3453f-110">Pregled programa Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="3453f-111">Pregled identitete in upravljanja dostopa v programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="3453f-112">Uvod v izgradnjo aplikacij Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="3453f-113">**Microsoft Graph Explorer** – preskusite API-je za Microsoft Graph v najemniku ali v demonstracijskem najemniku</span><span class="sxs-lookup"><span data-stu-id="3453f-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="3453f-114">**Želim uporabiti Microsoft Graph, vendar ne podpira API-jev imenika v 1.0, ki jih potrebujem?**</span><span class="sxs-lookup"><span data-stu-id="3453f-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="3453f-115">Microsoft Graph je priporočen API za imenik, identiteto in upravljanje dostopa.</span><span class="sxs-lookup"><span data-stu-id="3453f-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="3453f-116">Vendar pa še vedno obstaja nekaj vrzeli med tem, kar je mogoče v storitvi Azure AD Graph in Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3453f-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="3453f-117">Preglejte te članke, ki poudarjajo najbolj posodobljene razlike, ki jih boste lažje izbrali:</span><span class="sxs-lookup"><span data-stu-id="3453f-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="3453f-118">Razlike med vrstami virov med grafikonom Azure AD Graph in programom Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="3453f-119">Razlike med lastnostmi in grafikoni za Azure AD Graph in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="3453f-120">Razlike v metodi med storitvijo Azure AD in Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="3453f-121">**Ko poizvedujem po predmetu *uporabnika* , manjkajo številne njegove lastnosti**</span><span class="sxs-lookup"><span data-stu-id="3453f-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="3453f-122">`GET https://graph.microsoft.com/v1.0/users` vrne le 11 lastnosti, saj Microsoft Graph samodejno izbere privzeti nabor *uporabniških* lastnosti za vrnitev.</span><span class="sxs-lookup"><span data-stu-id="3453f-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="3453f-123">Če potrebujete druge lastnosti *uporabnika* , uporabite $SELECT, da izberete lastnosti, ki jih potrebuje vaš program.</span><span class="sxs-lookup"><span data-stu-id="3453f-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="3453f-124">Najprej preskusite v **programu Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="3453f-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="3453f-125">**Nekatere vrednosti lastnosti uporabnika so *ničelne* , čeprav vem, da so nastavljene**</span><span class="sxs-lookup"><span data-stu-id="3453f-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="3453f-126">Najbolj verjetna razlaga je, da je bila aplikacija dodeljena *uporabniku. ReadBasic. vse* dovoljenje.</span><span class="sxs-lookup"><span data-stu-id="3453f-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="3453f-127">S tem lahko program prebere omejen nabor uporabniških lastnosti, vrne vse druge lastnosti kot NULL, tudi če so bile prej nastavljene.</span><span class="sxs-lookup"><span data-stu-id="3453f-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="3453f-128">Poskusite podeliti *uporabnika aplikacije. preberi. vse* dovoljenje namesto tega.</span><span class="sxs-lookup"><span data-stu-id="3453f-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="3453f-129">Če želite več informacij, glejte [uporabniška dovoljenja za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="3453f-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="3453f-130">**Imam težave z uporabo parametrov poizvedbe OData za filtriranje podatkov v mojih zahtevah**</span><span class="sxs-lookup"><span data-stu-id="3453f-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="3453f-131">Medtem ko Microsoft Graph podpira širok spekter parametrov OData poizvedbe, številni od teh parametrov niso v celoti podprti s imeniškimi storitvami (viri, ki dedujejo od *directoryObject*) v programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3453f-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="3453f-132">Enake omejitve, ki so bile predstavljene v grafu Azure AD, se večinoma pojavljajo v programu Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="3453f-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="3453f-133">**Ni podprto**: $count, $search in *$filter v vrednosti null* ali *NOT NULL*</span><span class="sxs-lookup"><span data-stu-id="3453f-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="3453f-134">**Ni podprto**: $filter v določenih lastnostih (glejte teme vira, ki jih je treba filtrirati)</span><span class="sxs-lookup"><span data-stu-id="3453f-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="3453f-135">**Ni podprto**: ostranjevanje, filtriranje in razvrščanje hkrati</span><span class="sxs-lookup"><span data-stu-id="3453f-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="3453f-136">**Ni podprto**: filtriranje v relaciji.</span><span class="sxs-lookup"><span data-stu-id="3453f-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="3453f-137">Na primer – poiščite vse člane inženirske skupine, ki so v Združenem kraljestvu.</span><span class="sxs-lookup"><span data-stu-id="3453f-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="3453f-138">**Delna podpora**: $OrderBy na *uporabnika* (le displayName in userPrincipalName) in *skupino*</span><span class="sxs-lookup"><span data-stu-id="3453f-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="3453f-139">**Delna podpora**: $filter (podpira *le EQ*, *startswith*, or *in Limited* *) podpora*, $Expand (razširitev relacije posameznega predmeta vrne vse relacije, vendar pa je razširitev zbirke predmetov» relacija «omejena) </span><span class="sxs-lookup"><span data-stu-id="3453f-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="3453f-140">Če želite več informacij, glejte [prilagajanje odgovorov s parametri poizvedbe](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3453f-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="3453f-141">**Klic API, ki ga kličem, ne deluje – kje lahko naredim več testiranj?**</span><span class="sxs-lookup"><span data-stu-id="3453f-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="3453f-142">**Microsoft Graph Explorer** – preskusite API-je za Microsoft Graph v najemnika ali demonstracijskega najemnika in preverite **vzorčne poizvedbe** v Raziskovalcu programa Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3453f-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="3453f-143">**Ko poiščem podatke, se zdi, kot da dobim nedokončan nabor podatkov**</span><span class="sxs-lookup"><span data-stu-id="3453f-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="3453f-144">Če poizvedujete po zbirki (kot so *Uporabniki*), Microsoft Graph uporabi omejitve strani strežnika, tako da so rezultati vedno vrnjeni s privzeto velikostjo strani.</span><span class="sxs-lookup"><span data-stu-id="3453f-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="3453f-145">Program mora vedno pričakovati, da se bo stran povrnila prek zbirk, vrnjenih iz storitve.</span><span class="sxs-lookup"><span data-stu-id="3453f-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="3453f-146">Za več informacij glejte:</span><span class="sxs-lookup"><span data-stu-id="3453f-146">For more information, see:</span></span>

- [<span data-ttu-id="3453f-147">Najboljše prakse v programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="3453f-148">Ostranjevanje podatkov v aplikaciji Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="3453f-149">**Aplikacija je prepočasna in je tudi zadaviti. Katere izboljšave lahko izvedem?**</span><span class="sxs-lookup"><span data-stu-id="3453f-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="3453f-150">Odvisno od vašega scenarija je na voljo več različnih možnosti, s katerimi lahko izboljšate svojo aplikacijo in v nekaterih primerih zmanjšate možnost za omejevanje storitve (ko vnašate preveč klicev).</span><span class="sxs-lookup"><span data-stu-id="3453f-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="3453f-151">Več informacij nadete v tem članku:</span><span class="sxs-lookup"><span data-stu-id="3453f-151">To learn more, see:</span></span>

- [<span data-ttu-id="3453f-152">Najboljše prakse v programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="3453f-153">Zahteve za betonarne</span><span class="sxs-lookup"><span data-stu-id="3453f-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="3453f-154">Sledenja spremembam prek poizvedbe Delta</span><span class="sxs-lookup"><span data-stu-id="3453f-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="3453f-155">Pridobivanje obvestil o spremembah s pomočjo</span><span class="sxs-lookup"><span data-stu-id="3453f-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="3453f-156">Usmerjanje zadaviti</span><span class="sxs-lookup"><span data-stu-id="3453f-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="3453f-157">**Kje lahko najdem več informacij o napakah in znanih težavah?**</span><span class="sxs-lookup"><span data-stu-id="3453f-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="3453f-158">Informacije o odgovoru na Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="3453f-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="3453f-159">Znane težave z Microsoft Graphom</span><span class="sxs-lookup"><span data-stu-id="3453f-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="3453f-160">**Kje lahko preverim stanje razpoložljivosti storitve in povezljivosti?**</span><span class="sxs-lookup"><span data-stu-id="3453f-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="3453f-161">Razpoložljivost storitve in povezljivost osnovnih storitev, do katerih lahko dostopate prek Microsoft Grapha, lahko vpliva na splošno razpoložljivost in učinkovitost delovanja programa Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="3453f-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="3453f-162">Za zdravje storitve Azure Active Directory preverite stanje storitve **Security + Identity** Services, ki so navedene na [strani stanja Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="3453f-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="3453f-163">Za Officeove storitve, ki prispevajo k programu Microsoft Graph, preverite stanje storitev, ki so navedene v [nadzorni plošči» zdravstvena služba za Office](https://portal.office.com/adminportal/home#/servicehealth)«.</span><span class="sxs-lookup"><span data-stu-id="3453f-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
