---
title: Težave s povezavami in URL-ji
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707898"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="c45fe-102">Težave s povezavami in URL-ji</span><span class="sxs-lookup"><span data-stu-id="c45fe-102">Issues with links and URLs</span></span>

<span data-ttu-id="c45fe-103">URL-ji preusmeritve/odgovora (oba izraza sta izmenljiva) so URL-ji, ki jih Microsoftova platforma za identitete uporablja za vrnitev žetonov, zahtevanih s programom.</span><span class="sxs-lookup"><span data-stu-id="c45fe-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="c45fe-104">Če želite informacije o teh URL-jih, glejte te članke:</span><span class="sxs-lookup"><span data-stu-id="c45fe-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="c45fe-105">[Pretoki preverjanja pristnosti in scenariji uporabe](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – informacije o URL-jih preusmeritve na strani za registracijo **aplikacije** posameznega scenarija.</span><span class="sxs-lookup"><span data-stu-id="c45fe-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="c45fe-106">Omejitve URL-ja preusmeritve/odgovora</span><span class="sxs-lookup"><span data-stu-id="c45fe-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="c45fe-107">**Ne vem, kako registrirati pravi URI preusmeritve/URL za odgovor za svoj program**</span><span class="sxs-lookup"><span data-stu-id="c45fe-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="c45fe-108">Če se ob vpisu z aplikacijo, ki jo razvijate, prikaže pogovorno okno za vpis **AADSTS50011: URL za odgovor, ki je naveden v zahtevi, se ne ujema z URL-ji za odgovore, konfiguriranimi za aplikacijo <your app ID>**, boste morali dodati k registraciji programa, URI za preusmerjanje, ki ga je koda, uporabljena v zahtevi žetona, za Microsoftovo platformo za identitete.</span><span class="sxs-lookup"><span data-stu-id="c45fe-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="c45fe-109">Če želite dodati URL za odgovor, pojdite na zavihek **Authentication** na strani za registracijo aplikacije **v portalu Azure** dodajte vnos v razdelek **Redirect URL** (Preusmeri URL-je).</span><span class="sxs-lookup"><span data-stu-id="c45fe-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="c45fe-110">Vrednost, ki jo morate vnesti, je odvisna od vrste programa, ki ga gradite, kot je opisano spodaj:</span><span class="sxs-lookup"><span data-stu-id="c45fe-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="c45fe-111">Pri programih z eno stranjo in spletnih aplikacijah je URL odgovora URL v vaši aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="c45fe-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="c45fe-112">Oglejte [Registracija eno stran programa](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) ali [Registracija spletnega programa s portalom Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="c45fe-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="c45fe-113">Za namizne programe je vrednost, ki jo morate izbrati, odvisna od:</span><span class="sxs-lookup"><span data-stu-id="c45fe-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="c45fe-114">platforma (MacOS se razlikuje od sistema Windows ali Linux)</span><span class="sxs-lookup"><span data-stu-id="c45fe-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="c45fe-115">način pridobivanja žetona (interaktivno s tokom kode naprave, z integriranim preverjanjem pristnosti sistema Windows [IWA] ali z uporabniškim imenom/geslom).</span><span class="sxs-lookup"><span data-stu-id="c45fe-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="c45fe-116">Če želite več podrobnosti, glejte [namizne aplikacije – registracija aplikacije – Preusmerjanje URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="c45fe-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="c45fe-117">Za mobilne aplikacije je URI preusmeritve odvisen od tega:</span><span class="sxs-lookup"><span data-stu-id="c45fe-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="c45fe-118">platforma (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="c45fe-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="c45fe-119">informacije, uporabljene za ustvarjanje aplikacije, kot je ID svežnja v sistemu iOS, ter ime paketa in razdvoji podpis v sistemu Android Registracija aplikacije v portalu Azure vam bo pomagala.</span><span class="sxs-lookup"><span data-stu-id="c45fe-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="c45fe-120">Podrobnosti najdete v [konfiguracije platforme in preusmeritve URL-jev](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="c45fe-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="c45fe-121">Spletni API-ji in nekateri tihi načini pridobivanja žetonov (IWA in uporabniško ime/geslo) ne zahtevajo URI-ja preusmeritve.</span><span class="sxs-lookup"><span data-stu-id="c45fe-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="c45fe-122">**Uvedel sem spletni program in ko preskusim uvedeno aplikacijo, se prikaže sporočilo o ne spletnem naslovu za odgovor**</span><span class="sxs-lookup"><span data-stu-id="c45fe-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="c45fe-123">Dodajte URL-je preusmeritve za vsa mesta, na katerih uvajate spletni program.</span><span class="sxs-lookup"><span data-stu-id="c45fe-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="c45fe-124">Če želite več informacij, glejte [Registracija spletnega programa s portalom Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="c45fe-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="c45fe-125">URI preusmeritve za mesto dodajte takoj, ko uvedete program na tem mestu.</span><span class="sxs-lookup"><span data-stu-id="c45fe-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="c45fe-126">**Ne morem registrirati dovolj URL-jev za odgovor**</span><span class="sxs-lookup"><span data-stu-id="c45fe-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="c45fe-127">Ste ISV in imate enega ali več URL-jev za preusmerjanje za vsako stranko.</span><span class="sxs-lookup"><span data-stu-id="c45fe-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="c45fe-128">Iz storitve ADAL/Azure AD v1.0 želite preseliti v platformo za identitete MSAL/Microsoft in pri tem morate [največje dovoljeno število URL-jev za preusmeritev](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="c45fe-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="c45fe-129">To težavo odpravite tako, [dodate URL-je preusmeritve k glavnim](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), ki ustrezajo vsaki posamezni stranki.</span><span class="sxs-lookup"><span data-stu-id="c45fe-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
