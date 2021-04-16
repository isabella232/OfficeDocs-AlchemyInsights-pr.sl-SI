---
title: Med preverjanjem veljavnosti žetona za dostop med storitvijo Desktop Analytics na tabli je prišlo do napake
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813704"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="9d91e-102">Napaka »Pri sprejemanju žetona za dostop je prišlo do napake«</span><span class="sxs-lookup"><span data-stu-id="9d91e-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="9d91e-103">Ta napaka je običajno opazovana, ko poteče žeton za preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="9d91e-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="9d91e-104">Če osvežite stran, osvežite žeton.</span><span class="sxs-lookup"><span data-stu-id="9d91e-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="9d91e-105">Vendar pa lahko ta težava še vedno obstaja, če obstajajo pravilniki pogojnega dostopa, uporabljeni za račun, ki se uporablja za namizno analitiko na tabli.</span><span class="sxs-lookup"><span data-stu-id="9d91e-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="9d91e-106">Na portalu Azure Portal si lahko ogledate dnevnike vpisa v Azure AD in si ogledate, ali je prišlo do napak pri vpisu za račun, ki se uporablja za vpis v Namizno analitiko.</span><span class="sxs-lookup"><span data-stu-id="9d91e-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="9d91e-107">Če želite več informacij o pogojnem dostopu, [obiščite spletno mesto Načrtovanje uvajanja pogojnega dostopa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="9d91e-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>