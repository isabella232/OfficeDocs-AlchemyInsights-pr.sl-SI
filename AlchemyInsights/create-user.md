---
title: Ustvarjanje uporabnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569763"
---
# <a name="create-user"></a><span data-ttu-id="bbadb-102">Ustvarjanje uporabnika</span><span class="sxs-lookup"><span data-stu-id="bbadb-102">Create user</span></span>

<span data-ttu-id="bbadb-103">**OBVESTILO:**</span><span class="sxs-lookup"><span data-stu-id="bbadb-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="bbadb-104">[Zastaranje podpore za vpis v WebView v Googlu od 4. januarja 2021.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="bbadb-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="bbadb-105">Preverite, ali lahko na vaše aplikacije vplivajo [Googlova navodila](https://go.microsoft.com/fwlink/?linkid=2157323) za preskušanje združljivosti.</span><span class="sxs-lookup"><span data-stu-id="bbadb-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="bbadb-106">Poskrbite, da boste za vpis uporabnikov s potrošniškimi Google računi uporabljali sistemski spletni pogled ali brskalnik sistema.</span><span class="sxs-lookup"><span data-stu-id="bbadb-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="bbadb-107">Če želite več informacij, glejte [Težave pri vpisu v aplikacije le z brskalnikom Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="bbadb-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="bbadb-108">**Ne morem ustvariti novega uporabnika v imeniku Azure AD**</span><span class="sxs-lookup"><span data-stu-id="bbadb-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="bbadb-109">Prepričajte se, da imate dovoljenje za ustvarjanje novega standardnega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="bbadb-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="bbadb-110">Nov standardni uporabnik lahko ustvari le vloga globalnega skrbnika ali Azure Active Directory skrbnika v programu Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="bbadb-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="bbadb-111">Če niste v eni od teh vlog, prosite skrbnika, da vas doda na eno od teh vlog ali ustvari nov uporabniški račun za vas.</span><span class="sxs-lookup"><span data-stu-id="bbadb-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="bbadb-112">Zagotovite, da je uporabniško ime v domeni, ki je potrjena v imeniku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bbadb-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="bbadb-113">Če v imeniku Azure AD ni potrjenih imen domen po meri, lahko uporabite začetno domeno Azure AD, ki se konča z \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="bbadb-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="bbadb-114">Zagotovite, da je uporabniško ime v domeni, ki ni v domeni Azure AD iz imenika AD na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="bbadb-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="bbadb-115">Uporabnikov ni mogoče dodati v oblak z imeni domen, ki so povezana z domenami na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="bbadb-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="bbadb-116">Zagotovite, da noben drug uporabnik ali stik še nima uporabniškega imena, ki ga želite dodeliti novemu uporabniku.</span><span class="sxs-lookup"><span data-stu-id="bbadb-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="bbadb-117">Uporabniška imena morajo biti enolična v imeniku Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bbadb-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="bbadb-118">Glejte [Vloge in skrbniki imenika Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bbadb-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="bbadb-119">Oglejte si [imena domen](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) za Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bbadb-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="bbadb-120">Preglejte [dnevnike nadzora in](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) si oglejte podrobnejše informacije o nedavno ustvarjenem ali izbrisanem uporabniku, na primer o tem, kdo je izvedel dejanje in kdaj.</span><span class="sxs-lookup"><span data-stu-id="bbadb-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="bbadb-121">Če želite več informacij o dodajanju novih uporabnikov, glejte Uporaba portala Azure za [ustvarjanje novega uporabnika v imeniku Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="bbadb-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="bbadb-122">[Skrbniške vloge za Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)Skrbniška dovoljenja za vloge v Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="bbadb-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="bbadb-123">Novega uporabnika lahko ustvarite tudi z azure [AD PowerShell.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="bbadb-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
