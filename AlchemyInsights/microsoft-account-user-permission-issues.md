---
title: Odpravljanje težav – uporabnika ni bilo mogoče najti v imeniku
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725423"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="785e8-102">Odpravljanje težav – uporabnika ni bilo mogoče najti v imeniku</span><span class="sxs-lookup"><span data-stu-id="785e8-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="785e8-103">Če uporabniki prejmejo sporočilo o napaki» uporabnika ni mogoče najti «v imeniku, poskusite znova, kjer je vrsta težave uporabnik, ki ni v imeniku.</span><span class="sxs-lookup"><span data-stu-id="785e8-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="785e8-104">Če želite odpraviti težavo, se lahko dokončate s temi koraki.</span><span class="sxs-lookup"><span data-stu-id="785e8-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="785e8-105">Zagotovite, da je račun, ki je sprejel e-poštno povabilo, isti račun, ki se uporablja za vpis pozneje.</span><span class="sxs-lookup"><span data-stu-id="785e8-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="785e8-106">Prepričajte se, da uporabnik uporablja isti račun, da sprejme povabilo in se vpiše na mesto.</span><span class="sxs-lookup"><span data-stu-id="785e8-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="785e8-107">Če želite več informacij, glejte [upravljanje vzdevkov za Microsoftov račun </a> za upravljanje prijave v Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="785e8-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="785e8-108">Poiščite vsako mesto (-e), v katerem uporabnik prejme napako.</span><span class="sxs-lookup"><span data-stu-id="785e8-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="785e8-109">Dodajte»/_layouts/15/People.aspx/membershipgroupid = 0 «(znotraj dvojnih narekovajev) na konec URL-ja mesta.</span><span class="sxs-lookup"><span data-stu-id="785e8-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="785e8-110">Primer: https://<» contoso «>. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="785e8-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="785e8-111">Izberite uporabnika s seznama.</span><span class="sxs-lookup"><span data-stu-id="785e8-111">Select the user from the list.</span></span>

- <span data-ttu-id="785e8-112">Kliknite **Odstrani uporabniška dovoljenja** na traku.</span><span class="sxs-lookup"><span data-stu-id="785e8-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="785e8-113">Dodajte uporabnika in znova pošljite povabilo uporabniku.</span><span class="sxs-lookup"><span data-stu-id="785e8-113">Add back the User and Resend the invite to the user.</span></span>

