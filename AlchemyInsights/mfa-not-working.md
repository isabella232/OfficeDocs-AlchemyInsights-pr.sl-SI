---
title: Težave z MFP
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545197"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="82e6e-102">Težave z MFP</span><span class="sxs-lookup"><span data-stu-id="82e6e-102">Issues with MFA</span></span>
<span data-ttu-id="82e6e-103">So nekaj stvari v ček če uporabnik ne morem prepričevalnost using mnogo-činitelj Authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="82e6e-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="82e6e-104">Prizadeti uporabnik je morda blokiran v portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="82e6e-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="82e6e-105">V tem primeru bodo poskusi preverjanja pristnosti za tega določenega uporabnika samodejno zavrnjeni.</span><span class="sxs-lookup"><span data-stu-id="82e6e-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="82e6e-106">Prosimo, upoštevajte navodila v tem članku, da jih odblokirate.</span><span class="sxs-lookup"><span data-stu-id="82e6e-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="82e6e-107">Če odblokiranje uporabnik didnt ' pomoč ali uporabnik ni tnalo vi moči začeti v prikrivati MFA zakaj uporabnik ter oni hoteti iti skozi vpisati proces še.</span><span class="sxs-lookup"><span data-stu-id="82e6e-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="82e6e-108">Prosimo, upoštevajte navodila v tem članku.</span><span class="sxs-lookup"><span data-stu-id="82e6e-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="82e6e-109">Če to je prvi čas vi usposobiti MFA ter vaš uporabnik ste nezmožen v prepričevalnost v non-browsers varovanci kot na primer razgled, Skype, etc, morda ADAL (dejanje naslovnik Authentication knjižnica) ni usposobiti naprej vaš O365 abomna.</span><span class="sxs-lookup"><span data-stu-id="82e6e-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="82e6e-110">V tem primeru boste morali povezati z PowerShell Exchange Online in zaženite to cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="82e6e-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>