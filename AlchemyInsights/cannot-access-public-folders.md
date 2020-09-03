---
title: Dostop do javnih map ni mogoč
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341419"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="180e5-102">Outlook se ne more povezati z javnimi mapami</span><span class="sxs-lookup"><span data-stu-id="180e5-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="180e5-103">Če dostop do javne mape ne deluje za nekatere uporabnike, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="180e5-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="180e5-104">Povežite se s EKSO PowerShell in konfigurirajte parameter DefaultPublicFolderMailbox v uporabniškem računu težave, da se ujema s parametrom v delujočem uporabniškem računu.</span><span class="sxs-lookup"><span data-stu-id="180e5-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="180e5-105">Primer</span><span class="sxs-lookup"><span data-stu-id="180e5-105">Example:</span></span>

<span data-ttu-id="180e5-106">Get-poštni nabiralnik WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="180e5-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="180e5-107">Nastavitev nabiralnika ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="180e5-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="180e5-108">Počakajte vsaj eno uro, da sprememba začne veljati.</span><span class="sxs-lookup"><span data-stu-id="180e5-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="180e5-109">Če težava ostane, upoštevajte [ta postopek](https://aka.ms/pfcte) , da odpravite težave z dostopom do javnih map z Outlookom.</span><span class="sxs-lookup"><span data-stu-id="180e5-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="180e5-110">**Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map z Outlookom**:</span><span class="sxs-lookup"><span data-stu-id="180e5-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="180e5-111">Uporabite ukaz» Set-CASMailbox <mailboxname> -PublicFolderClientAccess «$TRUE ali $FALSE</span><span class="sxs-lookup"><span data-stu-id="180e5-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="180e5-112">$true: Omogočanje uporabnikom dostop do javnih map v Outlooku</span><span class="sxs-lookup"><span data-stu-id="180e5-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="180e5-113">$false: preprečite uporabniku dostop do javnih map v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="180e5-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="180e5-114">To je privzeta vrednost.</span><span class="sxs-lookup"><span data-stu-id="180e5-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="180e5-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="180e5-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="180e5-116">**Opomba** S tem postopkom lahko nadzorujete povezave le s programom Outlook Desktop za odjemalce sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="180e5-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="180e5-117">Uporabnik lahko še naprej dostopa do javnih map s programom OWA ali Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="180e5-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="180e5-118">Če želite več informacij, glejte [objava podpore za nadzorovane povezave z javnimi mapami v Outlooku](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="180e5-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>