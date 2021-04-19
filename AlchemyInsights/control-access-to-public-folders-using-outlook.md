---
title: Nadzor dostopa do javnih map z Outlookom
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816756"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="8548d-102">Nadzor dostopa do javnih map z Outlookom</span><span class="sxs-lookup"><span data-stu-id="8548d-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="8548d-103">Če želite nadzorovati, kateri uporabniki lahko dostopajo do javnih map v Outlooku:</span><span class="sxs-lookup"><span data-stu-id="8548d-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="8548d-104">Uporaba `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="8548d-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="8548d-105">$true: Omogočanje dostopa uporabnikom do javnih map v Outlooku</span><span class="sxs-lookup"><span data-stu-id="8548d-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="8548d-106">$false: Preprečite uporabnikom dostop do javnih map v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="8548d-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="8548d-107">To je privzeta vrednost.</span><span class="sxs-lookup"><span data-stu-id="8548d-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="8548d-108">Opomba: S tem postopkom lahko nadzorujete le povezave z namiznimi odjemalci za Outlook za Windows.</span><span class="sxs-lookup"><span data-stu-id="8548d-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="8548d-109">Uporabniki lahko še naprej dostopajo do javnih map s programom OWA ali Outlook for Mac.</span><span class="sxs-lookup"><span data-stu-id="8548d-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="8548d-110">Če želite več informacij, glejte [Nadzorovane povezave z javnimi mapami v Outlooku.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="8548d-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
