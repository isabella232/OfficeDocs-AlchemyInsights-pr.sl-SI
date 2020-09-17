---
title: Omogočanje arhivskega nabiralnika
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811722"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="82169-102">Omogočanje arhivskega nabiralnika</span><span class="sxs-lookup"><span data-stu-id="82169-102">Enable an archive mailbox</span></span>

<span data-ttu-id="82169-103">Če želite, da zaženemo avtomatizirane čeke, s katerimi zagotovite, da je lahko konfiguriran nabiralnik arhiva, izberite gumb» Vrni < «na vrhu te strani in nato vnesite e-poštni naslov računa.</span><span class="sxs-lookup"><span data-stu-id="82169-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="82169-104">Arhivski nabiralniki v programu Microsoft 365 (imenovani tudi *spletni arhivi* ali *Arhivi na*mestu uporabe) uporabnikom nudijo dodatno e-poštno shrambo.</span><span class="sxs-lookup"><span data-stu-id="82169-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="82169-105">Uporabniki lahko premaknejo ali kopirajo elemente v svoj arhivski nabiralnik, skrbniki pa lahko ustvarijo pravilnik arhiviranja, ki samodejno premakne elemente v arhivske nabiralnike.</span><span class="sxs-lookup"><span data-stu-id="82169-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="82169-106">Oglejte si navodila za ustvarjanje nabiralnika arhiva:</span><span class="sxs-lookup"><span data-stu-id="82169-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="82169-107">Pojdite na [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="82169-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="82169-108">Vpišite se v Microsoft 365 s skrbniškim računom.</span><span class="sxs-lookup"><span data-stu-id="82169-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="82169-109">V levem podoknu središča za skladnost z varnostjo &amp; Izberite Arhiv za **upravljanje informacij** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="82169-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="82169-110">Izberite uporabnika, čigar arhivski nabiralnik želite omogočiti.</span><span class="sxs-lookup"><span data-stu-id="82169-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="82169-111">V podoknu s podrobnostmi na desni strani kliknite **Omogoči** in nato kliknite **da** v opozorilnem sporočilu, da omogočite arhivski nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="82169-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="82169-112">Nabiralnike arhiva lahko tudi v razsutem stanju omogočite tako, da izberete več uporabnikov (s tipkama **SHIFT** ali **CTRL** ) in nato kliknete **Omogoči** v podoknu s podrobnostmi.</span><span class="sxs-lookup"><span data-stu-id="82169-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="82169-113">Nabiralniki v skupni rabi</span><span class="sxs-lookup"><span data-stu-id="82169-113">Shared mailboxes</span></span>

<span data-ttu-id="82169-114">Če želite omogočiti Arhiv za nabiralnik v skupni rabi, potrebujete licenco za Exchange Online (paket 2) ali licenco Exchange Online za paket 1 z licenco za arhiviranje v storitvi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="82169-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="82169-115">Če želite omogočiti Arhiv za nabiralnik v skupni rabi:</span><span class="sxs-lookup"><span data-stu-id="82169-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="82169-116">Pojdite v [skrbniško središče za Exchange](https://outlook.office365.com/ecp) in se vpišite s skrbniškim računom.</span><span class="sxs-lookup"><span data-stu-id="82169-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="82169-117">Pojdite na **prejemnike**  >  **v skupni rabi**.</span><span class="sxs-lookup"><span data-stu-id="82169-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="82169-118">Izberite nabiralnik v skupni rabi.</span><span class="sxs-lookup"><span data-stu-id="82169-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="82169-119">V podoknu s podrobnostmi na desni strani **v razdelku Arhiv na mestu**kliknite **Omogoči**in nato še **da** , da omogočite arhivski nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="82169-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="82169-120">Če želite več informacij, si oglejte:</span><span class="sxs-lookup"><span data-stu-id="82169-120">For more information, see:</span></span>
  
- [<span data-ttu-id="82169-121">Omogočanje arhivskih nabiralnikov</span><span class="sxs-lookup"><span data-stu-id="82169-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="82169-122">Nastavitev pravilnika o arhiviranju in brisanju</span><span class="sxs-lookup"><span data-stu-id="82169-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
