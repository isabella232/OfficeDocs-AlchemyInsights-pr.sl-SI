---
title: Težave z uporabo skrbniške konzole Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555878"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="046f1-102">Težave z uporabo skrbniške konzole Intune</span><span class="sxs-lookup"><span data-stu-id="046f1-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="046f1-103">**»Dostop zavrnjen« pri krmarjenju po skrbniškem portalu Intune.**</span><span class="sxs-lookup"><span data-stu-id="046f1-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="046f1-104">Če ste član vloge po meri Intune, se prepričajte, da je licenca EMS (Intune ali Enterprise Mobility Suite) dodeljena vašemu računu.</span><span class="sxs-lookup"><span data-stu-id="046f1-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="046f1-105">Če za upravljanje naprav uporabljate upravitelja konfiguracije, preverite, ali niste del uporabniške zbirke Intune za MDM upravitelja konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="046f1-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="046f1-106">Preverite, ali so vam bila v rezilu »Vloge Intune« dodeljena ustrezna dovoljenja za nadzor skrbništva na podlagi vlog (RBAC).</span><span class="sxs-lookup"><span data-stu-id="046f1-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="046f1-107">Preverite, ali uporabljena skupina ni seznam prejemnikov.</span><span class="sxs-lookup"><span data-stu-id="046f1-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="046f1-108">Intune v portalu Azure podpira samo uporabniške račune, ki pripadajo varnostnim skupinam storitve Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="046f1-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="046f1-109">Preglejte skupine v portalu Azure > **Intune**  >  **Groups**ali v portalu Azure > **imeniku Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="046f1-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="046f1-110">**Uporabnik ima preveč dovoljenj za dodeljeno vlogo Intune**</span><span class="sxs-lookup"><span data-stu-id="046f1-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="046f1-111">Svetujte uporabniku, da gre **v vloge Intune**  >  **Intune**  >  **Moja dovoljenja**  >  **Izvozi,** da pregleda odobrena dovoljenja.</span><span class="sxs-lookup"><span data-stu-id="046f1-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="046f1-112">**Vlogi sem dodal skupino obsegov, vendar uporabniki v tej vlogi še vedno vidijo druge uporabnike ali naprave.**</span><span class="sxs-lookup"><span data-stu-id="046f1-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="046f1-113">Skupine obsega ne filtrirajo uporabnikov ali naprav.</span><span class="sxs-lookup"><span data-stu-id="046f1-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="046f1-114">Skupine obsegov:</span><span class="sxs-lookup"><span data-stu-id="046f1-114">Scope groups:</span></span>

- <span data-ttu-id="046f1-115">Omejite, komu lahko uporabniki dodelijo pravilnike ali aplikacije.</span><span class="sxs-lookup"><span data-stu-id="046f1-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="046f1-116">Dovoli samo določenim uporabnikom, da izvajajo oddaljena opravila v napravah.</span><span class="sxs-lookup"><span data-stu-id="046f1-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="046f1-117">Če želite več informacij o skupinah obsega, [glejte Nadzor dostopa do vlog (RBAC) z Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="046f1-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="046f1-118">**Dodal sem uporabnika intune vlogo, vendar so še vedno popoln dostop do intune admin konzolo.**</span><span class="sxs-lookup"><span data-stu-id="046f1-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="046f1-119">Pomaknite se do možnosti Intune > **Uporabniki** v portalu Azure in preverite, ali uporabnik ni dodeljen nobeni od teh vlog v portalu Azure:</span><span class="sxs-lookup"><span data-stu-id="046f1-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="046f1-120">Globalni skrbnik</span><span class="sxs-lookup"><span data-stu-id="046f1-120">Global administrator</span></span>
- <span data-ttu-id="046f1-121">Skrbnik storitve Intune</span><span class="sxs-lookup"><span data-stu-id="046f1-121">Intune service administrator</span></span>
- <span data-ttu-id="046f1-122">Skrbnik SharePointa</span><span class="sxs-lookup"><span data-stu-id="046f1-122">SharePoint administrator</span></span>

<span data-ttu-id="046f1-123">Če želite več informacij, [glejte Nadzor dostopa po vlogi (RBAC) z MicrosoftOm Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="046f1-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="046f1-124">**Težave z dostopom**</span><span class="sxs-lookup"><span data-stu-id="046f1-124">**Access Issues**</span></span>

<span data-ttu-id="046f1-125">Če želite več informacij, [glejte Ne morete se vpisati v Office 365, Azure ali Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="046f1-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>