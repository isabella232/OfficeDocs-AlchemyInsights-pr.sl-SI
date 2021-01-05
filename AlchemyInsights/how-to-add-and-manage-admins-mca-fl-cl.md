---
title: Dodajanje in upravljanje skrbnikov
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
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755527"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="e4b56-102">Dodajanje in upravljanje skrbnikov</span><span class="sxs-lookup"><span data-stu-id="e4b56-102">How to add and manage admins</span></span>

<span data-ttu-id="e4b56-103">Na podlagi opisa vprašanja smo našli rešitev za vas.</span><span class="sxs-lookup"><span data-stu-id="e4b56-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="e4b56-104">Večina kupcev je lahko svojo težavo razrešila sami po tem, ko je sledila naši dokumentaciji.</span><span class="sxs-lookup"><span data-stu-id="e4b56-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="e4b56-105">Če želite upravljati račun obračunavanja za Microsoftovo stranko (MCA), lahko uporabite različne vloge z želeno ravnjo dostopa.</span><span class="sxs-lookup"><span data-stu-id="e4b56-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="e4b56-106">Te vloge so poleg vgrajenih vlog storitve Azure, ki vam pomagajo nadzorovati vire.</span><span class="sxs-lookup"><span data-stu-id="e4b56-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="e4b56-107">**Če želite dodati vloge za obračunavanje v portalu Azure:**</span><span class="sxs-lookup"><span data-stu-id="e4b56-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="e4b56-108">Vpišite se v [portal Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e4b56-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="e4b56-109">Poiščete *stroške Management + obračunavanje*.</span><span class="sxs-lookup"><span data-stu-id="e4b56-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="e4b56-110">Izberite nadzor dostopa (IAM) na obsegu, kot je račun za obračunavanje, profil obračunavanja ali odsek računa, kamor želite omogočiti dostop.</span><span class="sxs-lookup"><span data-stu-id="e4b56-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="e4b56-111">Na strani za nadzor dostopa (IAM) so navedeni uporabniki in skupine, ki so dodeljene vsaki vlogi za ta obseg.</span><span class="sxs-lookup"><span data-stu-id="e4b56-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="e4b56-112">Če želite omogočiti dostop do uporabnika, na vrhu strani izberite **Dodaj** .</span><span class="sxs-lookup"><span data-stu-id="e4b56-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="e4b56-113">Na spustnem seznamu *vloga* Izberite vlogo.</span><span class="sxs-lookup"><span data-stu-id="e4b56-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="e4b56-114">Vnesite e-poštni naslov uporabnika, ki mu želite omogočiti dostop.</span><span class="sxs-lookup"><span data-stu-id="e4b56-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="e4b56-115">Izberite **Shrani** , da dodelite vlogo.</span><span class="sxs-lookup"><span data-stu-id="e4b56-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="e4b56-116">Če želite odstraniti dostop za uporabnika, izberite uporabnika z dodeljeno vlogo, ki jo želite odstraniti.</span><span class="sxs-lookup"><span data-stu-id="e4b56-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="e4b56-117">Izberite **Odstrani**.</span><span class="sxs-lookup"><span data-stu-id="e4b56-117">Select **Remove**.</span></span>

<span data-ttu-id="e4b56-118">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="e4b56-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="e4b56-119">Definicije vloge za obračunavanje</span><span class="sxs-lookup"><span data-stu-id="e4b56-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="e4b56-120">Vloge in opravila obračunavanja računov</span><span class="sxs-lookup"><span data-stu-id="e4b56-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="e4b56-121">Začnite uporabljati račun za obračunavanje MCA</span><span class="sxs-lookup"><span data-stu-id="e4b56-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="e4b56-122">Preverjanje dostopa do Microsoftove pogodbe s strankami</span><span class="sxs-lookup"><span data-stu-id="e4b56-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
