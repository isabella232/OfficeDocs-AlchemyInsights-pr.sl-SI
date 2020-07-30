---
title: Premikanje e-poštnih sporočil v nabiralnik arhiviranja
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522787"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="c1580-102">Premikanje e-pošte v arhivski nabiralnik</span><span class="sxs-lookup"><span data-stu-id="c1580-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="c1580-103">Če želite, da zaženemo samodejne preglede za spodaj navedene nastavitve, izberite gumb za nazaj < - na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave pri premikanju e-pošte v svoj arhivski nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="c1580-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="c1580-104">Preverite, ali **je bil nabiralnik** arhiva omogočen.</span><span class="sxs-lookup"><span data-stu-id="c1580-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="c1580-105">Če ne, uporabite korake v [tem članku,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da omogočite arhivski nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="c1580-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="c1580-106">Če želite samodejno arhivirati sporočila v arhivski nabiralnik, mora biti oznaka hranjenja **z dejanjem »Premakni** v arhiv« nastavljena na **samodejno uporabljeno za celotno oznako nabiralnika (privzeto).**</span><span class="sxs-lookup"><span data-stu-id="c1580-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="c1580-107">Če želite ustvariti oznako: Arhiv privzete oznake [uporabite tukaj](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="c1580-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="c1580-108">Nato v pravilnik o **hranjenju** dodajte oznako Arhiv.</span><span class="sxs-lookup"><span data-stu-id="c1580-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="c1580-109">V Skrbniškem središču za Exchange izberite **Pravilniki** o hranjenju > dodajte **oznako Premakni** v arhiv v pravilnik > **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="c1580-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="c1580-110">Zdaj [dodelite pravilnik o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nabiralniku določenega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="c1580-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="c1580-111">Enak pravilnik bo uporabljen za nabiralnik **»Primarni« in** **»Arhiv«.**</span><span class="sxs-lookup"><span data-stu-id="c1580-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="c1580-112">Morda bo treba pomočnika za upravljane mape (MFA) prisiliti, da zažene in uporabi nove nastavitve v uporabnikovem nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="c1580-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="c1580-113">Ko ste povezani z lupino [EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) zaženite ta ukaz, da zaženete pomočnika za upravljane mape za določen nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="c1580-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="c1580-114">Start-ManagedFolderAssistant -Identiteta<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="c1580-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="c1580-115">Če želite več informacij o nastavitvi pravilnika arhiva, [glejte Nastavitev pravilnika arhiva in brisanja nabiralnikov](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="c1580-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  