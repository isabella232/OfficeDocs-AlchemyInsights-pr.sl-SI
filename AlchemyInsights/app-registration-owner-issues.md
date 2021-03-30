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
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405321"
---
# <a name="app-registration-owner-issues"></a>Težave lastnika registracije aplikacije

Spodaj so načini, kako lahko dodate glavnice kot lastnike za registracije aplikacij:

- Uporaba modula Azure AD PowerShell –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Sklic: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Uporaba storitve Azure CLI – `az ad app owner add`

    Sklic: [lastnik aplikacije az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Uporaba funkcije MS Graph –

    Sklic: [Dodajanje lastnika – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Uporaba portala Azure AD – premaknite se v [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App Registration > Izberite program, > Lastniki > Dodaj lastnike

**Si ne morete ogledati programa v reji registracije aplikacij, čeprav ste lastnik tega programa?**

Lastnik aplikacije ni skrbniška vloga. Če je nastavitev [Omeji dostop do skrbniškega portala](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) za Azure AD omogočena, si bodo aplikacije na portalu za registracijo aplikacije lahko ogledoli samo skrbniki. Če želite lastniku omogočiti ogled programov, onemogočite to nastavitev (Nastavite jo na NE) ali pa dodelite skrbniško vlogo lastniku le za določen program. Vendar pa boste za to potrebovali licenco za Azure AD Premium P2 in omogočili možnost [privilegiranem upravljanju identitet.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
