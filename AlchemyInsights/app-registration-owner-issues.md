---
title: Težave lastnika registracije aplikacije
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
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951149"
---
# <a name="app-registration-owner-issues"></a>Težave lastnika registracije aplikacije

Spodaj so načini, kako lahko dodate glavnice kot lastnike za registracije aplikacij:

- Uporaba modula Azure AD PowerShell –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Sklic: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Uporaba storitve Azure CLI – `az ad app owner add`

    Sklic: [lastnik aplikacije az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Uporaba MS Graph –

    Sklic: [Dodajanje lastnika – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Uporaba portala Azure AD – premaknite se v [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App Registration > Izberite program, > Lastniki > Dodaj lastnike

**Si ne morete ogledati programa v reji registracije aplikacij, čeprav ste lastnik tega programa?**

Lastnik aplikacije ni skrbniška vloga. Če je nastavitev [Omeji dostop do skrbniškega portala](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) za Azure AD omogočena, si bodo aplikacije na portalu za registracijo aplikacije lahko ogledoli samo skrbniki. Če želite lastniku omogočiti ogled programov, onemogočite to nastavitev (Nastavite jo na NE) ali pa dodelite skrbniško vlogo lastniku le za določen program. Za to pa boste potrebovali licenco za Azure AD Premium P2 in omogočite [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
