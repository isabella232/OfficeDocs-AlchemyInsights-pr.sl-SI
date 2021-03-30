---
title: Pridobite seznam programov za podjetja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405512"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="4c7be-102">Pridobite seznam programov za podjetja</span><span class="sxs-lookup"><span data-stu-id="4c7be-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="4c7be-103">Če **želite** dobiti seznam poslovnih aplikacij (vse aplikacije ali filtrirane po prikazanem imenu, ID-ju, URI-jih identifikatorja itd.) z ukazom Powershell, glejte [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span><span class="sxs-lookup"><span data-stu-id="4c7be-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="4c7be-104">Če želite z ukazom Powershell dobiti seznam glavnih predmetov storitve (vsi predmeti ali filtrirani po ID-ju), glejte [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)</span><span class="sxs-lookup"><span data-stu-id="4c7be-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="4c7be-105">Če želite dobiti **seznam programčkov, konfiguriranih s skripti SAML, si lahko** pomagate s skripti PowerShell:</span><span class="sxs-lookup"><span data-stu-id="4c7be-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="4c7be-106">Vsaka aplikacija je aplikacija OAuth ali saml (tako galerija kot tudi aplikacija, ki ni galerija) bi ob registraciji imela dva predmeta ustvarjena v AAD.</span><span class="sxs-lookup"><span data-stu-id="4c7be-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="4c7be-107">En predmet se imenuje Predmet programa, drugi pa je predmet Glavno ime storitve.</span><span class="sxs-lookup"><span data-stu-id="4c7be-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="4c7be-108">Ko z lupino PowerShell izvozite lastnosti glavnega predmeta storitve, ugotovite, da ima vsak program določeno število oznak, ki so povezane z njim:</span><span class="sxs-lookup"><span data-stu-id="4c7be-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="4c7be-109">Aplikacije OAuth imajo oznako, imenovano "**WindowsAzureActiveDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="4c7be-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="4c7be-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="4c7be-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="4c7be-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="4c7be-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="4c7be-112">Zato lahko te oznake uporabite in ugotovite, kakšna vrsta aplikacije je to.</span><span class="sxs-lookup"><span data-stu-id="4c7be-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="4c7be-113">Oznaka "**WindowsAzureActiveDirectoryIntegratedApp**" se uporablja za vse vrste aplikacij.</span><span class="sxs-lookup"><span data-stu-id="4c7be-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="4c7be-114">Ta izrezek lahko uporabite za seznam vseh aplikacij SAML (tako galerije kot tudi iz galerije):</span><span class="sxs-lookup"><span data-stu-id="4c7be-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="4c7be-115">Če želite več informacij, glejte [Prepoznavanje aplikacij, ki omogočajo SAML, v imeniku Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="4c7be-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="4c7be-116">Iskanje in **seznam le spletnih programov:** Uporabite spodnji ukaz, če želite vse aplikacije Azure AD pisati z vrsto programa »Spletna aplikacija/API«</span><span class="sxs-lookup"><span data-stu-id="4c7be-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="4c7be-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="4c7be-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="4c7be-118">**Samo poiščite in navedite izvorne** aplikacije: Zaženite ta ukaz, da pridobite vse izvorne odjemalske programe (namizne/prenosne naprave).</span><span class="sxs-lookup"><span data-stu-id="4c7be-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="4c7be-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="4c7be-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="4c7be-120">**Izvoz vseh registriranih podrobnosti programa Azure AD v DATOTEKO CSV:** S spodnjim ukazom izvozite vse aplikacije Azure AD z zahtevanimi podrobnostmi v datoteko CSV:</span><span class="sxs-lookup"><span data-stu-id="4c7be-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="4c7be-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="4c7be-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="4c7be-122">Export-Csv »C:\AzureADApps.csv« -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="4c7be-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="4c7be-123">**Izvoz seznama neuporabljenih aplikacij Azure** – poročilo o nadzoru</span><span class="sxs-lookup"><span data-stu-id="4c7be-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="4c7be-124">Azure AD lahko dnevnike aplikacij prikaže le do 30 dni, če imate licenco za Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="4c7be-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="4c7be-125">Podatke lahko hranite dlje kot 30 dni na dva dni.</span><span class="sxs-lookup"><span data-stu-id="4c7be-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="4c7be-126">Z [API-ji za poročanje Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) lahko programsko pridobite podatke in jih shranite v zbirko podatkov.</span><span class="sxs-lookup"><span data-stu-id="4c7be-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="4c7be-127">Lahko pa tudi integrigrite dnevnike nadzora v sistem SIEM drugega strani.</span><span class="sxs-lookup"><span data-stu-id="4c7be-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="4c7be-128">Prav tako lahko prenesete seznam aplikacij za vse aplikacije in aplikacije v lasti v razdelku Azure Active Directory>Registracije aplikacij>Download>All applications/Owned applications.</span><span class="sxs-lookup"><span data-stu-id="4c7be-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="4c7be-129">Če želite dobiti seznam aplikacij s storitvijo MS Graph, glejte Aplikacije seznama [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) in vrsta vira aplikacije [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span><span class="sxs-lookup"><span data-stu-id="4c7be-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
