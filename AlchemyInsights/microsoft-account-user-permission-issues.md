---
title: Odpravljanje težav – uporabnik ni bil najden v imeniku
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702754"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="e199f-102">Odpravljanje težav – uporabnik ni bil najden v imeniku</span><span class="sxs-lookup"><span data-stu-id="e199f-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="e199f-103">Če uporabnik ste sprejemanje zmota vest "uporabnik vekanje ' obstati ustanavljati" v naslovnik, prosim začeti še kraj izdaja stavek je uporabnik ne v naslovnik.</span><span class="sxs-lookup"><span data-stu-id="e199f-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="e199f-104">Za odpravljanje težave je mogoče dokončati naslednje korake.</span><span class="sxs-lookup"><span data-stu-id="e199f-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="e199f-105">Zagotovite, da je račun, ki je sprejel e-poštno povabilo, isti račun, ki se uporablja za vpis pozneje.</span><span class="sxs-lookup"><span data-stu-id="e199f-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="e199f-106">Prepričajte se, da uporabnik uporablja isti račun, da sprejme povabilo in se prijavite v spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="e199f-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="e199f-107">Če želite več informacij, glejte [upravljanje vzdevkov za svoj Microsoftov račun</a> za upravljanje Microsoftove 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="e199f-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="e199f-108">Prebrskajte do vsakega mesta (-ov), v katerem uporabnik prejema napako.</span><span class="sxs-lookup"><span data-stu-id="e199f-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="e199f-109">Dodaj "/_layouts/15/People.aspx/membershipgroupid = 0" (znotraj dvojne narekovaje) do konca URL-ja spletnega mesta.</span><span class="sxs-lookup"><span data-stu-id="e199f-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="e199f-110">Primer: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="e199f-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="e199f-111">Izberite uporabnika s seznama.</span><span class="sxs-lookup"><span data-stu-id="e199f-111">Select the user from the list.</span></span>

- <span data-ttu-id="e199f-112">Kliknite **Odstrani uporabniške pravice** s traku.</span><span class="sxs-lookup"><span data-stu-id="e199f-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="e199f-113">Dodajte nazaj uporabnika in ponovno Pošlji povabilo uporabniku.</span><span class="sxs-lookup"><span data-stu-id="e199f-113">Add back the User and Resend the invite to the user.</span></span>

