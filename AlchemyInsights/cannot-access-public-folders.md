---
title: Dostop do javnih map ni na voljo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819528"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="f46bd-102">Outlook se ne more povezati z javnimi mapami</span><span class="sxs-lookup"><span data-stu-id="f46bd-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="f46bd-103">Če dostop do javnih map ne deluje za nekatere uporabnike, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="f46bd-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="f46bd-104">Vzpostavite povezavo z exo PowerShell in konfigurirajte parameter DefaultPublicFolderMailbox za težaveni uporabniški račun, da se bo ujemal s parametrom v delovnem uporabniškem računu.</span><span class="sxs-lookup"><span data-stu-id="f46bd-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="f46bd-105">Primer:</span><span class="sxs-lookup"><span data-stu-id="f46bd-105">Example:</span></span>

<span data-ttu-id="f46bd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="f46bd-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="f46bd-107">Set-Mailbox TežavaUporabnik -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="f46bd-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="f46bd-108">Počakajte vsaj eno uro, da sprememba začne veljati.</span><span class="sxs-lookup"><span data-stu-id="f46bd-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="f46bd-109">Če težave ne odpravite, upoštevajte ta [postopek](https://aka.ms/pfcte) in odpravite težave z dostopom do javnih map z Outlookom.</span><span class="sxs-lookup"><span data-stu-id="f46bd-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="f46bd-110">**Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map v Outlooku:**</span><span class="sxs-lookup"><span data-stu-id="f46bd-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="f46bd-111">Uporabite Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ali $false</span><span class="sxs-lookup"><span data-stu-id="f46bd-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="f46bd-112">$true: Omogočanje dostopa uporabnikom do javnih map v Outlooku</span><span class="sxs-lookup"><span data-stu-id="f46bd-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="f46bd-113">$false: Preprečite uporabnikom dostop do javnih map v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="f46bd-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="f46bd-114">To je privzeta vrednost.</span><span class="sxs-lookup"><span data-stu-id="f46bd-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="f46bd-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="f46bd-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="f46bd-116">**Opomba** S tem postopkom lahko nadzorujete povezave le z namiznim programom Outlook za Windows.</span><span class="sxs-lookup"><span data-stu-id="f46bd-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="f46bd-117">Uporabnik lahko še naprej dostopa do javnih map s programom OWA ali Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="f46bd-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="f46bd-118">Če želite več informacij, [glejte Napove najavljena podpora za nadzorovane povezave do javnih map v Outlooku.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="f46bd-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>