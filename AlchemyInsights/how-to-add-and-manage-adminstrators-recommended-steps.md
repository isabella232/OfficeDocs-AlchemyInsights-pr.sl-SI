---
title: Kako dodati in upravljati adminstrators – priporočene korake
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678871"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="c2d8e-102">Kako dodati in upravljati adminstrators – priporočene korake</span><span class="sxs-lookup"><span data-stu-id="c2d8e-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="c2d8e-103">**Urejanje upravitelja naročnine ali soskrbnika**</span><span class="sxs-lookup"><span data-stu-id="c2d8e-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="c2d8e-104">Skrbnik računa lahko ureja obe vlogi, medtem ko lahko skrbnik naročnine spremeni le soskrbnike v [portalu Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="c2d8e-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="c2d8e-105">Dodajanje ali spreminjanje skrbnikov naročnine na Azure</span><span class="sxs-lookup"><span data-stu-id="c2d8e-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="c2d8e-106">**Posodobitev skrbnika naročnine ali Co-Administrator za notranje (AIRS) naročnine**</span><span class="sxs-lookup"><span data-stu-id="c2d8e-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="c2d8e-107">Skrbnik storitve ali soskrbnik lahko to dejanje samouporabi s temi koraki:</span><span class="sxs-lookup"><span data-stu-id="c2d8e-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="c2d8e-108">Prijavite se v [portal Azure](https://ms.portal.azure.com/#home) in kliknite **upravljanje stroškov + obračunavanje** v levem rezilu.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="c2d8e-109">Kliknite element vrstice z naročnino.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="c2d8e-110">S tem odprete pregled naročnine.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="c2d8e-111">Na rezilu **naročnine** kliknite **lastnosti**.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="c2d8e-112">Kliknite gumb» **skrbnik storitve** «.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="c2d8e-113">Vnesite e-poštno sporočilo uporabnika, ki ga želite nastaviti kot skrbnika storitve, in kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="c2d8e-114">**Dodajanje/spreminjanje/odstranjevanje soskrbnika**</span><span class="sxs-lookup"><span data-stu-id="c2d8e-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="c2d8e-115">Prijavite se v [portal Azure](https://ms.portal.azure.com/#home) kot skrbnik storitve.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="c2d8e-116">Odpiranje [naročnin](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in izbiranje naročnine.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="c2d8e-117">(Adminstrators lahko dodelite le na obseg naročnine.)</span><span class="sxs-lookup"><span data-stu-id="c2d8e-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="c2d8e-118">Pomaknite se do razdelka» **nadzor dostopa «(iam) –**  >  **klasični skrbniki**  >  **dodajte**  >  **Dodajanje soskrbnika** , da odprete podokno **Dodajanje** soodločanja (če je možnost Dodaj soskrbnika onemogočena, to pomeni, da nimate dovoljenj).</span><span class="sxs-lookup"><span data-stu-id="c2d8e-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="c2d8e-119">Izberite uporabnika, ki ga želite dodati, in kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="c2d8e-120">**več:**</span><span class="sxs-lookup"><span data-stu-id="c2d8e-120">**Learn more:**</span></span>
- [<span data-ttu-id="c2d8e-121">Dodajanje soskrbnika</span><span class="sxs-lookup"><span data-stu-id="c2d8e-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="c2d8e-122">Odstranjevanje soskrbnika</span><span class="sxs-lookup"><span data-stu-id="c2d8e-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="c2d8e-123">Spreminjanje skrbnika storitve</span><span class="sxs-lookup"><span data-stu-id="c2d8e-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="c2d8e-124">Ogled skrbnika računa</span><span class="sxs-lookup"><span data-stu-id="c2d8e-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="c2d8e-125">Upravljanje dostopa s portalom» RBAC «in» Azure «</span><span class="sxs-lookup"><span data-stu-id="c2d8e-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="c2d8e-126">**Dodajanje/brisanje uporabnikov z imenikom Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="c2d8e-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="c2d8e-127">Dodate lahko nove uporabnike ali izbrišete obstoječe uporabnike iz organizacije Azure Active Directory (Azure AD):</span><span class="sxs-lookup"><span data-stu-id="c2d8e-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="c2d8e-128">Če želite dodati novega uporabnika, se prijavite v [portal Azure](https://ms.portal.azure.com/#home) kot uporabnik – skrbnik organizacije.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="c2d8e-129">Izberite **Azure Active Directory**, izberite **Uporabniki** in nato kliknite **nov uporabnik**.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="c2d8e-130">Na strani **uporabnik** izpolnite zahtevane informacije.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="c2d8e-131">Kliknite **Ustvari**.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-131">Click **Create**.</span></span> <span data-ttu-id="c2d8e-132">Uporabnik je ustvarjen in dodan v najemnika v storitvi Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c2d8e-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="c2d8e-133">**Več informacij**:</span><span class="sxs-lookup"><span data-stu-id="c2d8e-133">**Learn more**:</span></span>

- [<span data-ttu-id="c2d8e-134">Dodajanje novega uporabnika</span><span class="sxs-lookup"><span data-stu-id="c2d8e-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="c2d8e-135">Brisanje uporabnika</span><span class="sxs-lookup"><span data-stu-id="c2d8e-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="c2d8e-136">Dodajanje ali posodabljanje uporabnikovih podatkov profila v storitvi Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c2d8e-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="c2d8e-137">**Priporočeni dokumenti**</span><span class="sxs-lookup"><span data-stu-id="c2d8e-137">**Recommended documents**</span></span>

- [<span data-ttu-id="c2d8e-138">Kaj je nadzor dostopa na podlagi vloge (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="c2d8e-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="c2d8e-139">Razumevanje različnih vlog v storitvi Azure</span><span class="sxs-lookup"><span data-stu-id="c2d8e-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="c2d8e-140">Dovoljenja skrbnika za vlogo v imeniku Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c2d8e-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="c2d8e-141">Vadnica: dodeljevanje dostopa uporabniku z uporabo RBAC in portala Azure</span><span class="sxs-lookup"><span data-stu-id="c2d8e-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="c2d8e-142">Odpravljanje težav s RBAC v storitvi Azure</span><span class="sxs-lookup"><span data-stu-id="c2d8e-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="c2d8e-143">Organizirajte vire s skupinami za upravljanje Azure</span><span class="sxs-lookup"><span data-stu-id="c2d8e-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="c2d8e-144">Kako zaprositi ulitek od Azure račun pot email</span><span class="sxs-lookup"><span data-stu-id="c2d8e-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="c2d8e-145">Dodajanje, posodabljanje ali odstranjevanje kreditne ali debetne kartice v storitvi Azure</span><span class="sxs-lookup"><span data-stu-id="c2d8e-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="c2d8e-146">Upravljanje naročnine (vnovična aktivacija/preklic/preklop)</span><span class="sxs-lookup"><span data-stu-id="c2d8e-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



