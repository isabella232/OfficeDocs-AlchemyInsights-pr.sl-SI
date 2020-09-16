---
title: Selitev iz AIP v MIP/enotno označevanje v središču za skladnost
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674342"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="0305f-102">Selitev iz AIP v MIP/enotno označevanje v središču za skladnost</span><span class="sxs-lookup"><span data-stu-id="0305f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="0305f-103">Če želite preseliti iz oznak AIP na enotno označevanje v središču za varnost in skladnost s predpisi, naredite to:</span><span class="sxs-lookup"><span data-stu-id="0305f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="0305f-104">**Aktiviranje zaščite v portalu Azure**</span><span class="sxs-lookup"><span data-stu-id="0305f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="0305f-105">Če tega še niste storili, odprite novo okno brskalnika in se [vpišite v portal Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="0305f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="0305f-106">Pomaknite se do rezila za **zaščito informacij Azure** .</span><span class="sxs-lookup"><span data-stu-id="0305f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="0305f-107">V meniju zvezdišče na primer kliknite **vse storitve** in začnite vnašati **podatke** v polje filter.</span><span class="sxs-lookup"><span data-stu-id="0305f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="0305f-108">Izberite **zaščita za Azure Information**.</span><span class="sxs-lookup"><span data-stu-id="0305f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="0305f-109">Če še niste dostopali do rezila za zaščito informacij Azure, si oglejte enkratne [dodatne korake](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) za dodajanje tega rezila v portal.</span><span class="sxs-lookup"><span data-stu-id="0305f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="0305f-110">Če želite odpreti rezilo za zaščito informacij Azure, morate imeti [paket Premium za zaščito](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) informacij ali paket Office 365, ki vključuje upravljanje pravic.</span><span class="sxs-lookup"><span data-stu-id="0305f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="0305f-111">Če imate eno od teh naročnin, vendar se prikaže sporočilo, da ni mogoče najti veljavne naročnine, se [obrnite na Microsoftovo podporo](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) ali uporabite standardne kanale za podporo.</span><span class="sxs-lookup"><span data-stu-id="0305f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="0305f-112">Poiščite možnosti za **upravljanje** menija in izberite **aktivacija zaščite**.</span><span class="sxs-lookup"><span data-stu-id="0305f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="0305f-113">Kliknite **Aktiviraj**in potrdite dejanje.</span><span class="sxs-lookup"><span data-stu-id="0305f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="0305f-114">Ko je aktiviranje dokončano, vrstica z informacijami prikaže **uspešno dokončano aktiviranje**.</span><span class="sxs-lookup"><span data-stu-id="0305f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="0305f-115">**Selitev oznak za zaščito informacij Azure v Office 365 Security Center za skladnost s predpisi &**</span><span class="sxs-lookup"><span data-stu-id="0305f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="0305f-116">Prepričajte se, da ste prijavljeni kot uporabnik z dovoljenjem globalnega skrbnika.</span><span class="sxs-lookup"><span data-stu-id="0305f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="0305f-117">Pomaknite se do rezila za **zaščito informacij Azure** .</span><span class="sxs-lookup"><span data-stu-id="0305f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="0305f-118">V možnosti» **Upravljaj** meni «izberite **poenoteno označevanje**.</span><span class="sxs-lookup"><span data-stu-id="0305f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="0305f-119">Na rezilu z **oznako Azure Information-enotno označevanje** kliknite **Aktiviraj** in sledite spletnim navodilom.</span><span class="sxs-lookup"><span data-stu-id="0305f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="0305f-120">**Opomba**: Preverite, ali imate ustrezna dovoljenja, preden aktivirate selitveni center za skladnost varnostnega &.</span><span class="sxs-lookup"><span data-stu-id="0305f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="0305f-121">Če želite več informacij, si oglejte te članke:</span><span class="sxs-lookup"><span data-stu-id="0305f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="0305f-122">Ali morate biti globalni skrbnik, če želite konfigurirati zaščito informacij Azure ali lahko prenesem na druge skrbnike?</span><span class="sxs-lookup"><span data-stu-id="0305f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="0305f-123">Pomembne informacije o skrbniških vlogah po selitvi v središče za skladnost s predpisi o varnosti &.</span><span class="sxs-lookup"><span data-stu-id="0305f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="0305f-124">Če želite več informacij o AIP za poenoteno označevanje selitve v središče za varnost in skladnost s predpisi, glejte [selitev nalepk](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="0305f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
