---
title: Pravilniki za gesla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747053"
---
# <a name="password-policies"></a><span data-ttu-id="18e15-102">Pravilniki za gesla</span><span class="sxs-lookup"><span data-stu-id="18e15-102">Password policies</span></span>

<span data-ttu-id="18e15-103">**Imam težave s pravilnikom za gesla za uporabnika**</span><span class="sxs-lookup"><span data-stu-id="18e15-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="18e15-104">Pravilnik gesel za uporabnika je odvisen od tega, ali je uporabnik le v oblaku ali na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="18e15-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="18e15-105">Le uporabniki v oblaku morajo izbrati geslo, ki izpolnjuje zahteve v tem članku: [Pravilniki o geslih, ki veljajo le za uporabniške račune v oblaku](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="18e15-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="18e15-106">Uporabniki na mestu uporabe morajo izbrati geslo, ki izpolnjuje zahteve na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="18e15-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="18e15-107">Če uporabnik na mestu uporabe ne more nastaviti svojega gesla, preverite zahteve na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="18e15-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="18e15-108">**Ne vem, kako naj nastavim ali preverim pravilnike o poteku gesel**</span><span class="sxs-lookup"><span data-stu-id="18e15-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="18e15-109">Pravilnik o zapadlosti za uporabnike v oblaku v najemniku lahko nastavite in preverite z uporabo lupine PowerShell.</span><span class="sxs-lookup"><span data-stu-id="18e15-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="18e15-110">Sledite navodilom v tem članku: [nastavitev ali preverjanje pravilnikov gesel z uporabo lupine PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="18e15-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="18e15-111">Pravilnik o zapadlosti gesla za uporabnike na mestu uporabe je nastavljen v OGLASu na mestu uporabe.</span><span class="sxs-lookup"><span data-stu-id="18e15-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="18e15-112">**Druge uporabne povezave:**</span><span class="sxs-lookup"><span data-stu-id="18e15-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="18e15-113">Uvod v ponastavitev gesla</span><span class="sxs-lookup"><span data-stu-id="18e15-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="18e15-114">Odpravljanje težav s ponastavitvijo gesla za skrbnike</span><span class="sxs-lookup"><span data-stu-id="18e15-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
