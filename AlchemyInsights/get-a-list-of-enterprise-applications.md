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
# <a name="get-a-list-of-enterprise-applications"></a>Pridobite seznam programov za podjetja

1. Če **želite** dobiti seznam poslovnih aplikacij (vse aplikacije ali filtrirane po prikazanem imenu, ID-ju, URI-jih identifikatorja itd.) z ukazom Powershell, glejte [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Če želite z ukazom Powershell dobiti seznam glavnih predmetov storitve (vsi predmeti ali filtrirani po ID-ju), glejte [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Če želite dobiti **seznam programčkov, konfiguriranih s skripti SAML, si lahko** pomagate s skripti PowerShell:

    Vsaka aplikacija je aplikacija OAuth ali saml (tako galerija kot tudi aplikacija, ki ni galerija) bi ob registraciji imela dva predmeta ustvarjena v AAD. En predmet se imenuje Predmet programa, drugi pa je predmet Glavno ime storitve. Ko z lupino PowerShell izvozite lastnosti glavnega predmeta storitve, ugotovite, da ima vsak program določeno število oznak, ki so povezane z njim:

    - Aplikacije OAuth imajo oznako, imenovano "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Zato lahko te oznake uporabite in ugotovite, kakšna vrsta aplikacije je to. Oznaka "**WindowsAzureActiveDirectoryIntegratedApp**" se uporablja za vse vrste aplikacij. Ta izrezek lahko uporabite za seznam vseh aplikacij SAML (tako galerije kot tudi iz galerije):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Če želite več informacij, glejte [Prepoznavanje aplikacij, ki omogočajo SAML, v imeniku Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. Iskanje in **seznam le spletnih programov:** Uporabite spodnji ukaz, če želite vse aplikacije Azure AD pisati z vrsto programa »Spletna aplikacija/API«

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Samo poiščite in navedite izvorne** aplikacije: Zaženite ta ukaz, da pridobite vse izvorne odjemalske programe (namizne/prenosne naprave).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Izvoz vseh registriranih podrobnosti programa Azure AD v DATOTEKO CSV:** S spodnjim ukazom izvozite vse aplikacije Azure AD z zahtevanimi podrobnostmi v datoteko CSV:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv »C:\AzureADApps.csv« -NoTypeInformation -Encoding UTF8

7. **Izvoz seznama neuporabljenih aplikacij Azure** – poročilo o nadzoru

    Azure AD lahko dnevnike aplikacij prikaže le do 30 dni, če imate licenco za Azure AD Premium.
    Podatke lahko hranite dlje kot 30 dni na dva dni. Z [API-ji za poročanje Azure AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) lahko programsko pridobite podatke in jih shranite v zbirko podatkov. Lahko pa tudi integrigrite dnevnike nadzora v sistem SIEM drugega strani.

    Prav tako lahko prenesete seznam aplikacij za vse aplikacije in aplikacije v lasti v razdelku Azure Active Directory>Registracije aplikacij>Download>All applications/Owned applications.

    Če želite dobiti seznam aplikacij s storitvijo MS Graph, glejte Aplikacije seznama [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) in vrsta vira aplikacije [– Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
