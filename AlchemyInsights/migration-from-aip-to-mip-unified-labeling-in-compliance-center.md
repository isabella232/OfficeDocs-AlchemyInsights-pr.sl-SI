---
title: Selitev iz programa AIP v mip/poenoteno označevanje v središču za skladnost s predpisi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825387"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="045ca-102">Selitev iz programa AIP v mip/poenoteno označevanje v središču za skladnost s predpisi</span><span class="sxs-lookup"><span data-stu-id="045ca-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="045ca-103">Če želite oznake AIP preseliti v poenoteno označevanje v središču za varnost in skladnost s predpisi, naredite to:</span><span class="sxs-lookup"><span data-stu-id="045ca-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="045ca-104">**Aktiviranje zaščite s portala Azure**</span><span class="sxs-lookup"><span data-stu-id="045ca-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="045ca-105">Če tega še niste naredili, odprite novo okno brskalnika in se [vpišite v portal Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="045ca-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="045ca-106">Pomaknite se do **re žetice Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="045ca-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="045ca-107">V meniju zvezdišča na primer kliknite **Vse storitve** in začnite vnašati **Informacije** v polje Filter.</span><span class="sxs-lookup"><span data-stu-id="045ca-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="045ca-108">Izberite **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="045ca-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="045ca-109">Če še niste dostopali do re naročnine na Azure Information Protection, si oglejte enkratne dodatne korake za dodajanje [tega](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) re bladea v portal.</span><span class="sxs-lookup"><span data-stu-id="045ca-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="045ca-110">Če želite odpreti re naročnino za Azure Information Protection, morate imeti paket [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) ali paket storitve Office 365, ki vključuje storitev Rights Management.</span><span class="sxs-lookup"><span data-stu-id="045ca-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="045ca-111">Če imate eno od teh naročnin, vendar se prikaže sporočilo, da veljavne naročnine ni mogoče [najti,](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) se obrnite na Microsoftovo podporo ali uporabite standardne kanale podpore.</span><span class="sxs-lookup"><span data-stu-id="045ca-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="045ca-112">Poiščite možnosti **menija** Upravljanje in izberite **Zaščita za aktiviranje**.</span><span class="sxs-lookup"><span data-stu-id="045ca-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="045ca-113">Kliknite **Aktiviraj** in potrdite dejanje.</span><span class="sxs-lookup"><span data-stu-id="045ca-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="045ca-114">Po dokončanem aktiviranju je v vrstici z informacijami **prikazano, da je aktiviranje uspešno dokončano.**</span><span class="sxs-lookup"><span data-stu-id="045ca-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="045ca-115">**Selitev oznak Azure Information Protection v Središče za varnost in skladnost s predpisi storitve Office 365 & s predpisi**</span><span class="sxs-lookup"><span data-stu-id="045ca-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="045ca-116">Prepričajte se, da ste prijavljeni kot uporabnik z dovoljenjem globalnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="045ca-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="045ca-117">Pomaknite se do **re žetice Azure Information Protection.**</span><span class="sxs-lookup"><span data-stu-id="045ca-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="045ca-118">V **meniju** Upravljaj izberite **Poenoteno označevanje**.</span><span class="sxs-lookup"><span data-stu-id="045ca-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="045ca-119">V re **bladeu Azure Information Protection – poenoteno označevanje** kliknite **Aktiviraj** in upoštevajte spletna navodila.</span><span class="sxs-lookup"><span data-stu-id="045ca-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="045ca-120">**Opomba:** Preverite, ali imate ustrezna dovoljenja, preden aktivirate selitev središča za & s predpisi.</span><span class="sxs-lookup"><span data-stu-id="045ca-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="045ca-121">Več informacij najdete v teh člankih:</span><span class="sxs-lookup"><span data-stu-id="045ca-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="045ca-122">Ali morate biti globalni skrbnik, če želite konfigurirati Azure Information Protection, ali sem lahko pooblaščen drugim skrbnikom?</span><span class="sxs-lookup"><span data-stu-id="045ca-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="045ca-123">Pomembne informacije o skrbniških vlogah po selitvi v središče za & s predpisi.</span><span class="sxs-lookup"><span data-stu-id="045ca-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="045ca-124">Če želite več informacij o selitvi AIP v poenoteno označevanje v središče za varnost in skladnost s predpisi, glejte [Selitev oznak.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="045ca-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
