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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891765"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="4900d-102">Outlook ne more vzpostaviti povezave z javnimi mapami</span><span class="sxs-lookup"><span data-stu-id="4900d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="4900d-103">Če dostop do javne mape za nekatere uporabnike ne deluje, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="4900d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="4900d-104">Povežite se z lupino EXO in konfigurirajte parameter DefaultPublicFolderMailbox na uporabnikovem uporabniškem računu, da se ujema s parametrom v delovnem uporabniškem računu.</span><span class="sxs-lookup"><span data-stu-id="4900d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="4900d-105">Primer:</span><span class="sxs-lookup"><span data-stu-id="4900d-105">Example:</span></span>

<span data-ttu-id="4900d-106">Get-poštni nabiralnik WorkingUser | ft DefaultPublicFolderMailbox, Efetivepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="4900d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="4900d-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<vrednost iz prejšnjega ukaza></span><span class="sxs-lookup"><span data-stu-id="4900d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="4900d-108">Počakajte vsaj eno uro, da sprememba učinkuje.</span><span class="sxs-lookup"><span data-stu-id="4900d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="4900d-109">Če težava ostane, upoštevajte [ta postopek](https://aka.ms/pfcte) , če želite odpraviti težave z dostopom do javnih map z Outlookom.</span><span class="sxs-lookup"><span data-stu-id="4900d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>