---
title: Prišlo je do napake pri preverjanju napake pri dostopu do žetona v storitvi Desktop Analytics na
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741274"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="11eb7-102">"Prišlo je do napake pri preverjanju dostopa žetona" Napaka med Desktop Analytics uvajanje</span><span class="sxs-lookup"><span data-stu-id="11eb7-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="11eb7-103">Ta napaka je običajno opažena, ko žeton za preverjanje pristnosti poteče.</span><span class="sxs-lookup"><span data-stu-id="11eb7-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="11eb7-104">Običajno osveževanje strani Osveži žeton.</span><span class="sxs-lookup"><span data-stu-id="11eb7-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="11eb7-105">Vendar pa to vprašanje lahko traja, če obstajajo pravilniki o pogojnem dostopu, ki se uporabljajo za račun, ki se uporablja za namizno analitiko na vozilu.</span><span class="sxs-lookup"><span data-stu-id="11eb7-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="11eb7-106">V dnevnikih Azure AD Sign in v portalu Azure lahko preverite, ali obstajajo kakršne koli napake pri vpisu za račun, ki se uporablja za namizni Analytics.</span><span class="sxs-lookup"><span data-stu-id="11eb7-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="11eb7-107">Če želite več informacij o pogojnem dostopu, obiščite [načrtovanje uvajanja pogojnega dostopa](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="11eb7-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>