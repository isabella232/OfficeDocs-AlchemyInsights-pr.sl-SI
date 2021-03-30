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
# <a name="app-registration-owner-issues"></a><span data-ttu-id="cc7c4-102">Težave lastnika registracije aplikacije</span><span class="sxs-lookup"><span data-stu-id="cc7c4-102">App Registration Owner issues</span></span>

<span data-ttu-id="cc7c4-103">Spodaj so načini, kako lahko dodate glavnice kot lastnike za registracije aplikacij:</span><span class="sxs-lookup"><span data-stu-id="cc7c4-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="cc7c4-104">Uporaba modula Azure AD PowerShell –</span><span class="sxs-lookup"><span data-stu-id="cc7c4-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="cc7c4-105">Sklic: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="cc7c4-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="cc7c4-106">Uporaba storitve Azure CLI – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="cc7c4-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="cc7c4-107">Sklic: [lastnik aplikacije az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="cc7c4-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="cc7c4-108">Uporaba funkcije MS Graph –</span><span class="sxs-lookup"><span data-stu-id="cc7c4-108">Using MS Graph -</span></span>

    <span data-ttu-id="cc7c4-109">Sklic: [Dodajanje lastnika – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="cc7c4-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="cc7c4-110">Uporaba portala Azure AD – premaknite se v [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > App Registration > Izberite program, > Lastniki > Dodaj lastnike</span><span class="sxs-lookup"><span data-stu-id="cc7c4-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="cc7c4-111">**Si ne morete ogledati programa v reji registracije aplikacij, čeprav ste lastnik tega programa?**</span><span class="sxs-lookup"><span data-stu-id="cc7c4-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="cc7c4-112">Lastnik aplikacije ni skrbniška vloga.</span><span class="sxs-lookup"><span data-stu-id="cc7c4-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="cc7c4-113">Če je nastavitev [Omeji dostop do skrbniškega portala](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) za Azure AD omogočena, si bodo aplikacije na portalu za registracijo aplikacije lahko ogledoli samo skrbniki.</span><span class="sxs-lookup"><span data-stu-id="cc7c4-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="cc7c4-114">Če želite lastniku omogočiti ogled programov, onemogočite to nastavitev (Nastavite jo na NE) ali pa dodelite skrbniško vlogo lastniku le za določen program.</span><span class="sxs-lookup"><span data-stu-id="cc7c4-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="cc7c4-115">Vendar pa boste za to potrebovali licenco za Azure AD Premium P2 in omogočili možnost [privilegiranem upravljanju identitet.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="cc7c4-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
