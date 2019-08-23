---
title: Vprašanja z MZZ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545197"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="cd8b4-102">Vprašanja z MZZ</span><span class="sxs-lookup"><span data-stu-id="cd8b4-102">Issues with MFA</span></span>
<span data-ttu-id="cd8b4-103">Obstaja nekaj stvari, da preverite, če uporabnikov ne morete prijaviti z uporabo multi-overjanja (MFP)</span><span class="sxs-lookup"><span data-stu-id="cd8b4-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cd8b4-104">Uporabnikov lahko blokiran v Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="cd8b4-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cd8b4-105">Če je temu tako, preverjanje pristnosti poskusov za to določenega uporabnika bo samodejno zavrnjen.</span><span class="sxs-lookup"><span data-stu-id="cd8b4-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cd8b4-106">Prosimo, sledite korakom v tem članku, da jih odblokirate.</span><span class="sxs-lookup"><span data-stu-id="cd8b4-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cd8b4-107">Če deblokiranje uporabnik ni pomagalo ali uporabnik ni tnalo vi moči začeti vprikrivati MFP za uporabnika in bo šel skozi proces enroll spet.</span><span class="sxs-lookup"><span data-stu-id="cd8b4-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cd8b4-108">Prosimo, sledite korakom v tem članku.</span><span class="sxs-lookup"><span data-stu-id="cd8b4-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cd8b4-109">Če je prvič omogočena MZZ in uporabniki ste nezmožen v prepričevalnost-brskalniki stranke, kot so Outlook, Skype, itd, morda ADAL (Active Directory preverjanje pristnosti knjižnico) ni omogočen na naročnino O365.</span><span class="sxs-lookup"><span data-stu-id="cd8b4-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cd8b4-110">V tem primeru boste morali povezati Exchange Online Powershell in zaženite ukaz cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="cd8b4-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>