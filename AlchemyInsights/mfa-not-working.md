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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768853"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="ccc65-102">Težave s storitvijo Azure MFA</span><span class="sxs-lookup"><span data-stu-id="ccc65-102">Issues with Azure MFA</span></span>
<span data-ttu-id="ccc65-103">Obstaja nekaj stvari, ki jih je treba preveriti, če se uporabniki ne morejo prijaviti z uporabo večfaktorskega preverjanja pristnosti (MFP)</span><span class="sxs-lookup"><span data-stu-id="ccc65-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="ccc65-104">Prizadeti uporabnik je morda blokiran v portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ccc65-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="ccc65-105">V tem primeru bodo poskusi preverjanja pristnosti za tega določenega uporabnika samodejno zavrnjeni.</span><span class="sxs-lookup"><span data-stu-id="ccc65-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="ccc65-106">Prosimo, upoštevajte navodila v tem članku, da jih odblokirate.</span><span class="sxs-lookup"><span data-stu-id="ccc65-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="ccc65-107">Če odblokiranje uporabnik didnt ' pomoč ali uporabnik ni tnalo vi moči začeti v prikrivati MFA zakaj uporabnik ter oni hoteti iti skozi vpisati proces še.</span><span class="sxs-lookup"><span data-stu-id="ccc65-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="ccc65-108">Prosimo, upoštevajte navodila v tem članku.</span><span class="sxs-lookup"><span data-stu-id="ccc65-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="ccc65-109">Če to je prvi čas vi usposobiti MFA ter vaš uporabnik ste nezmožen v prepričevalnost v non-browsers varovanci kot na primer razgled, Skype, etc, morda ADAL (dejanje naslovnik Authentication knjižnica) ni usposobiti naprej vaš O365 abomna.</span><span class="sxs-lookup"><span data-stu-id="ccc65-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="ccc65-110">V tem primeru boste morali povezati z PowerShell Exchange Online in zaženite to cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="ccc65-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>