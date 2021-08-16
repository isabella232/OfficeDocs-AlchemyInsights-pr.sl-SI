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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098618"
---
# <a name="issues-with-azure-mfa"></a>Težave s storitvijo Azure MFA
Preverite lahko nekaj stvari, ali se uporabniki ne morejo prijaviti s storitvijo Multi-Factor Authentication (MFA)

1. Ta uporabnik je morda blokiran v Azure Active Directory Portalu. V tem primeru bo preverjanje pristnosti za tega določenega uporabnika samodejno zavrnjeno. [Upoštevajte navodila v tem članku, da jih deblokirate.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Če deblokiranje uporabnika ni pomagalo ali če uporabnik ni blokiran, poskusite ponastaviti storitev MFA za uporabnika in ta bo znova prestal postopek včlanitev. [Upoštevajte navodila v tem članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Če ste storitev Multi-Authentication omogočili prvič in se vaši uporabniki ne morejo prijaviti v odjemalce, ki niso brskalniki, kot so Outlook, Skype itd. V naročnini na O365 morda ni omogočena knjižnica ADAL (knjižnica preverjanja pristnosti imenika Active Directory). V tem primeru boste morali vzpostaviti povezavo z Exchange Online Powershell in zagnati ta ukaz »cmdlet«: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*