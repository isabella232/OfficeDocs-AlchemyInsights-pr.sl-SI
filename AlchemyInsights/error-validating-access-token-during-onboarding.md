---
title: Prišlo je do napake pri preverjanju napake pri dostopu do žetona med namizno analizo na tabli
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783567"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="c0c43-102">Napaka pri preverjanju žetona za dostop do napake pri namizni analitiki</span><span class="sxs-lookup"><span data-stu-id="c0c43-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="c0c43-103">Ta napaka se običajno opazi, ko poteče žeton za preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="c0c43-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="c0c43-104">Po navadi osveževanje strani Osveži žeton.</span><span class="sxs-lookup"><span data-stu-id="c0c43-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="c0c43-105">Vendar pa lahko ta težava traja, če obstajajo kakršne koli pravilnike za pogojni dostop, ki se uporabljajo za račun, ki se uporablja za namizno analizo na vozilu.</span><span class="sxs-lookup"><span data-stu-id="c0c43-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="c0c43-106">Če želite preveriti, ali obstajajo napake pri vpisu za račun, ki se uporablja za namizne analitike, lahko pregledate vpis v storitvi Azure AD v dnevnike v portalu Azure.</span><span class="sxs-lookup"><span data-stu-id="c0c43-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="c0c43-107">Če želite več informacij o pogojnem dostopu, obiščite [načrt za uvajanje pogojnega dostopa](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="c0c43-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>