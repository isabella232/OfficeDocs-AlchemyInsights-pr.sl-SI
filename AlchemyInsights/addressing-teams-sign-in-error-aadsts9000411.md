---
title: Naslavljanje napake pri vpisu v skupine AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358369"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="e1abb-102">Naslavljanje napake pri vpisu v skupine AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="e1abb-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="e1abb-103">Ko se vpišete v Microsoft Teams, se lahko prikaže napaka: **žal, vendar imamo težave s podpisom vas v AADSTS9000411: zahteva ni pravilno oblikovana. Parameter» login_hint «je podvojena.**</span><span class="sxs-lookup"><span data-stu-id="e1abb-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="e1abb-104">Če želite odpraviti to težavo, preverite, ali so vaši odjemalci Microsoft Teams posodobljeni.</span><span class="sxs-lookup"><span data-stu-id="e1abb-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="e1abb-105">Če želite več informacij o posodabljanju odjemalca, glejte [posodabljanje programa Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="e1abb-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="e1abb-106">Če ne morete posodobiti odjemalca iz neznanega razloga, odjavite odjemalca bo jasno večino predpomnjenih podatkov.</span><span class="sxs-lookup"><span data-stu-id="e1abb-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="e1abb-107">Vendar, če vi še vedno življati izdaja čez odjavo/samoznak, prenehati skupina ter prosim veder vaš varovanec cache z početje sledeč:</span><span class="sxs-lookup"><span data-stu-id="e1abb-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="e1abb-108">Zaprite Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="e1abb-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="e1abb-109">Pojdite na:%AppData%\microsoft\teams in izbrišite vse datoteke.</span><span class="sxs-lookup"><span data-stu-id="e1abb-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="e1abb-110">Znova odprite Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="e1abb-110">Reopen Microsoft Teams.</span></span>
