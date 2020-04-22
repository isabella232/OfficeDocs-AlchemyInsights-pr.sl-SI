---
title: Premikanje e-poštnih sporočil v arhivski nabiralnik
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713662"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="d5f11-102">Premakni e-poštno sporočilo v arhivski nabiralnik</span><span class="sxs-lookup"><span data-stu-id="d5f11-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="d5f11-103">Potrdite, da je bil omogočen **arhivski nabiralnik** .</span><span class="sxs-lookup"><span data-stu-id="d5f11-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="d5f11-104">Če ne, uporabite korake v [tem članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) , da omogočite arhivski nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="d5f11-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="d5f11-105">Če želite samodejno arhivirati sporočila v arhivski nabiralnik, mora biti oznaka za hranjenje z dejanjem **Premakni v arhiviranje** nastavljena tako, da se **samodejno uporabi za celoten nabiralnik (privzeta) oznaka**.</span><span class="sxs-lookup"><span data-stu-id="d5f11-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="d5f11-106">Uporabite korake tukaj za ustvarjanje oznake: [Arhiv privzeta oznaka](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="d5f11-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="d5f11-107">Nato dodajte **arhivsko** oznako v pravilnik o hranjenju.</span><span class="sxs-lookup"><span data-stu-id="d5f11-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="d5f11-108">V skrbniškem središču za Exchange izberite **Pravilniki o hranjenju** > dodajte **oznako Premakni v arhiv** v pravilnik > **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="d5f11-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="d5f11-109">Zdaj [dodelite pravilnik o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) za nabiralnik določenega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="d5f11-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="d5f11-110">Ista politika bo uporabljena za **primarni** in **arhivski** nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="d5f11-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="d5f11-111">Morda bo potrebno prisiliti pomočnika za upravljane mape (MFA), da zažene in uporabi nove nastavitve v nabiralniku uporabnika.</span><span class="sxs-lookup"><span data-stu-id="d5f11-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="d5f11-112">Zaženite ta ukaz, medtem ko je [povezan z lupino EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , da zaženete pomočnika za upravljane mape za določen nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="d5f11-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="d5f11-113">Start-ManagedFolderAssistant-identiteta<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="d5f11-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="d5f11-114">Če želite več informacij o nastavitvi pravilnika arhiva, glejte [nastavitev pravilnika o arhiviranju in brisanju nabiralnikov](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="d5f11-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  