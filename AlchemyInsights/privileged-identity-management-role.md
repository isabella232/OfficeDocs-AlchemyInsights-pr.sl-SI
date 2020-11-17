---
title: Prednostna vloga za upravljanje identitete
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089151"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="5b0fa-102">Vloga za upravljanje s privilegirano identiteto (PIM)</span><span class="sxs-lookup"><span data-stu-id="5b0fa-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="5b0fa-103">**Dovoljenja niso dodeljena po aktivaciji vloge**</span><span class="sxs-lookup"><span data-stu-id="5b0fa-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="5b0fa-104">Ko aktivirate vlogo v sistemu za upravljanje identitete v storitvi Azure AD (PIM), se aktiviranje morda ne bo takoj razširilo na vse portale, ki zahtevajo privilegirano vlogo.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="5b0fa-105">Tudi če je sprememba razširjena, lahko spletno predpomnjenje v portalu povzroči, da sprememba ne začne veljati takoj.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="5b0fa-106">Če je aktivacija odložena, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="5b0fa-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5b0fa-107">Izpišite se iz portala Azure in se nato znova vpišite.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="5b0fa-108">Ko aktivirate vlogo Azure AD ali vlogo Azure Resource, boste videli faze aktiviranja.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="5b0fa-109">Ko so vse faze dokončane, se prikaže povezava» izpis «.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="5b0fa-110">To povezavo lahko uporabite, če se želite izpisati. To bo rešilo večino primerov za zakasnitev aktiviranja.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="5b0fa-111">V storitvi PIM preverite, ali ste navedeni kot član vloge.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="5b0fa-112">Če aktivirate vlogo skrbnika strežnika Exchange, se prepričajte, da ste se odjavili in se znova prijavili.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="5b0fa-113">Če težave ne morete odpraviti, odprite vstopnico za podporo in jo dvignite kot težavo.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="5b0fa-114">Če uporabljate svojo vlogo skrbnika Exchangea za dostop do središča za varnost in skladnost s predpisi, glejte naslednji korak.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="5b0fa-115">Če aktivirate vlogo za dostop do središča za varnost in skladnost s predpisi ali če aktivirate vlogo skrbnika za SharePoint, boste nekaj minut odpravili z zakasnitvijo do nekaj ur.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="5b0fa-116">To je znana težava in aktivno sodelujemo s temi ekipami, da to težavo odpravimo čimprej.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="5b0fa-117">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="5b0fa-117">For more information, see:</span></span>

- [<span data-ttu-id="5b0fa-118">Aktiviranje vlog» Azure AD «v sistemu PIM</span><span class="sxs-lookup"><span data-stu-id="5b0fa-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="5b0fa-119">Aktivacija mojih vlog» Azure Resource «v PIM</span><span class="sxs-lookup"><span data-stu-id="5b0fa-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="5b0fa-120">**Dovoljenja niso odstranjena, ko deaktivirate vlogo ali pa poteče aktiviranje vloge**</span><span class="sxs-lookup"><span data-stu-id="5b0fa-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="5b0fa-121">Ko deaktivirate vlogo v privilegiranem upravljanju identitete v storitvi Azure AD ali ko poteče obdobje aktiviranja vloge, je morda prišlo do zakasnitve, kjer boste še naprej imeli dostop.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="5b0fa-122">Če je vaša Deaktivacija odložena, upoštevajte ta navodila:</span><span class="sxs-lookup"><span data-stu-id="5b0fa-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5b0fa-123">Če deaktivirate vlogo skrbnika strežnika Exchange ali poteče obdobje aktiviranja vloge, in opazite veliko zamudo, preden so dovoljenja odstranjena, odprite vstopnico za podporo in povejte inženirju za podporo, da vam pomaga vložiti vstopnico za ekipo za upravljanje privilegiranega dostopa (PAM) v storitvi Office o tej težavi.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="5b0fa-124">Če je obdobje aktiviranja poteklo, vendar imate še vedno odprto sejo brskalnika, zaprite brskalnik.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="5b0fa-125">Vlogo lahko še naprej uporabljate, dokler ne zaprete te seje.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="5b0fa-126">To je znana težava, ki jo lahko odpravite tako, da aktivno ukine vsako sejo, ko je aktiviranje poteklo.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="5b0fa-127">Če se zamuda razlikuje od teh dveh scenarijev, odprite vstopnico za podporo.</span><span class="sxs-lookup"><span data-stu-id="5b0fa-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
