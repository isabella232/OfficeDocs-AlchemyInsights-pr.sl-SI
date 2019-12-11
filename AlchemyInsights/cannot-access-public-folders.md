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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959510"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="98326-102">Outlook ne more vzpostaviti povezave z javnimi mapami</span><span class="sxs-lookup"><span data-stu-id="98326-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="98326-103">Če dostop do javne mape za nekaj uporabnikov ne deluje, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="98326-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="98326-104">Povežite se z lupino EXO PowerShell in konfigurirajte DefaultPublicFolderMailbox na težavi uporabniški račun, da se ujemajo z enim na delovnem uporabniškem računu.</span><span class="sxs-lookup"><span data-stu-id="98326-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="98326-105">Primer:</span><span class="sxs-lookup"><span data-stu-id="98326-105">Example:</span></span>

<span data-ttu-id="98326-106">Get-poštni nabiralnik WorkingUser | ft DefaultPublicFolderMailbox, Efetivepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="98326-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="98326-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<vrednost iz prejšnjega ukaza></span><span class="sxs-lookup"><span data-stu-id="98326-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="98326-108">Počakajte vsaj eno uro, da sprememba učinkuje.</span><span class="sxs-lookup"><span data-stu-id="98326-108">Wait at least one hour for the change to take effect.</span></span>