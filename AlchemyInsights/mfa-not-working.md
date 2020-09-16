---
title: Težave s storitvijo MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755147"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="2eedf-102">Težave s storitvijo Azure MFA</span><span class="sxs-lookup"><span data-stu-id="2eedf-102">Issues with Azure MFA</span></span>
<span data-ttu-id="2eedf-103">Če želite preveriti, ali se uporabniki ne morejo prijaviti z uporabo multi-Factor Authentication (MFA), lahko preverite nekaj stvari</span><span class="sxs-lookup"><span data-stu-id="2eedf-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="2eedf-104">Prizadeti uporabnik je lahko blokiran v portalu Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="2eedf-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="2eedf-105">Če je to res, bodo poskusi preverjanja pristnosti tega določenega uporabnika samodejno zavrnjeni.</span><span class="sxs-lookup"><span data-stu-id="2eedf-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="2eedf-106">Upoštevajte navodila v tem članku, da jih odblokirate.</span><span class="sxs-lookup"><span data-stu-id="2eedf-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="2eedf-107">Če deblokiranje uporabnika ni pomagalo ali uporabnik ni blokiran, lahko poskusite ponastaviti MFA za uporabnika in bodo znova vzpostavili postopek za včlanitev.</span><span class="sxs-lookup"><span data-stu-id="2eedf-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="2eedf-108">Upoštevajte navodila v tem članku.</span><span class="sxs-lookup"><span data-stu-id="2eedf-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="2eedf-109">Če je to prvič, da ste omogočili MFA in se vaši uporabniki ne morejo prijaviti v odjemalce, ki niso brskalniki, kot so Outlook, Skype itd., morda knjižnice ADAL (knjižnica za preverjanje pristnosti imenika Active Directory) ni omogočena v naročnini na O365.</span><span class="sxs-lookup"><span data-stu-id="2eedf-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="2eedf-110">V tem primeru se boste morali povezati s storitvijo Exchange Online PowerShell in zagnati ukaz» cmdlet «:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="2eedf-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>