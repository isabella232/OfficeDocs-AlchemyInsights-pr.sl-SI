---
title: Težave z MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810500"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="569de-102">Težave s storitvijo Azure MFA</span><span class="sxs-lookup"><span data-stu-id="569de-102">Issues with Azure MFA</span></span>
<span data-ttu-id="569de-103">Preverite lahko nekaj stvari, ali se uporabniki ne morejo prijaviti s storitvijo Multi-Factor Authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="569de-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="569de-104">Uporabnik, na katerega to vpliva, je morda blokiran v portalu za Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="569de-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="569de-105">V tem primeru bo preverjanje pristnosti za tega določenega uporabnika samodejno zavrnjeno.</span><span class="sxs-lookup"><span data-stu-id="569de-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="569de-106">Upoštevajte navodila v tem članku, da jih deblokirate.</span><span class="sxs-lookup"><span data-stu-id="569de-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="569de-107">Če deblokiranje uporabnika ni pomagalo ali če uporabnik ni blokiran, poskusite ponastaviti storitev MFA za uporabnika in ta bo znova prestal postopek včlanitev.</span><span class="sxs-lookup"><span data-stu-id="569de-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="569de-108">Upoštevajte navodila v tem članku.</span><span class="sxs-lookup"><span data-stu-id="569de-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="569de-109">Če ste storitev MFA prvič omogočili in se vaši uporabniki ne morejo prijaviti v odjemalce, ki niso brskalniki, kot je Outlook, Skype itd. V naročnini na O365 morda ni omogočena knjižnica ADAL (knjižnica preverjanja pristnosti imenika Active Directory).</span><span class="sxs-lookup"><span data-stu-id="569de-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="569de-110">V tem primeru se boste morali povezati s storitvijo Exchange Online Powershell in zagnati ta ukaz »cmdlet«:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="569de-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>