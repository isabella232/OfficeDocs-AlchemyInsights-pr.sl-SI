---
title: Brisanje najemnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564880"
---
# <a name="delete-tenant"></a><span data-ttu-id="c3626-102">Brisanje najemnika</span><span class="sxs-lookup"><span data-stu-id="c3626-102">Delete tenant</span></span>

<span data-ttu-id="c3626-103">Če želite izbrisati oglas Azure, zagotovite:</span><span class="sxs-lookup"><span data-stu-id="c3626-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="c3626-104">Ste globalni skrbnik v imeniku.</span><span class="sxs-lookup"><span data-stu-id="c3626-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="c3626-105">Niste vpisani z računom, ki ima privzeti imenik, kot je contoso.onmicrosoft.com, v računu, kot je na primer admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="c3626-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="c3626-106">Pred brisanjem odstranite vse aktivne aplikacije v imeniku.</span><span class="sxs-lookup"><span data-stu-id="c3626-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="c3626-107">Če želite odstraniti aktivne aplikacije, se pomaknite do registracij programov in odstranite obstoječe aplikacije.</span><span class="sxs-lookup"><span data-stu-id="c3626-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="c3626-108">Ni aktivnih naročnin za vse Microsoftove spletne storitve, kot je Microsoft Azure, Office 365 ali Azure AD Premium, ki je povezan v imeniku.</span><span class="sxs-lookup"><span data-stu-id="c3626-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="c3626-109">Prenesite naročnine ali pospešite preklic aktivnih naročnin prek storitve Azure support in obračunavanje.</span><span class="sxs-lookup"><span data-stu-id="c3626-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="c3626-110">Preberite več o tem, kako preklicati naročnine na Office 365 in Azure.</span><span class="sxs-lookup"><span data-stu-id="c3626-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="c3626-111">Če želite navodila za združevanje ali dodajanje obstoječe naročnine najemniku, [si oglejte povezovanje ali dodajanje naročnine na AZURE ad najemniku](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="c3626-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="c3626-112">Ni aktivne licence.</span><span class="sxs-lookup"><span data-stu-id="c3626-112">There are no Active license.</span></span> <span data-ttu-id="c3626-113">Če želite odstraniti licence, si oglejte [Kako odstranite naročnino, da odstranite licenco](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="c3626-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="c3626-114">Pri poskusu brisanja Azure AD ni nobenega drugega aktivnega uporabnika v imeniku poleg samega sebe kot globalnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="c3626-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="c3626-115">Odstranite vse druge aktivne uporabnike, zato je treba odstraniti tudi vse odvisnosti v imenu domene po meri v najemniku, kot so uporabniki, ustvarjeni z admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c3626-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="c3626-116">Če želite več podrobnosti o tem, kako:</span><span class="sxs-lookup"><span data-stu-id="c3626-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="c3626-117">Izbrišite» imenik Azure Active Directory «ali» naročnina «, glejte [brisanje imenika Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="c3626-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="c3626-118">Če želite odstraniti aplikacije v imeniku, glejte [odstranjevanje programov](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="c3626-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
