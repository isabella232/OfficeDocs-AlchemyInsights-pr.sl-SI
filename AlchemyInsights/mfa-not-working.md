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
# <a name="issues-with-azure-mfa"></a>Težave s storitvijo Azure MFA
Preverite lahko nekaj stvari, ali se uporabniki ne morejo prijaviti s storitvijo Multi-Factor Authentication (MFA)

1. Uporabnik, na katerega to vpliva, je morda blokiran v portalu za Azure Active Directory. V tem primeru bo preverjanje pristnosti za tega določenega uporabnika samodejno zavrnjeno. [Upoštevajte navodila v tem članku, da jih deblokirate.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Če deblokiranje uporabnika ni pomagalo ali če uporabnik ni blokiran, poskusite ponastaviti storitev MFA za uporabnika in ta bo znova prestal postopek včlanitev. [Upoštevajte navodila v tem članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Če ste storitev MFA prvič omogočili in se vaši uporabniki ne morejo prijaviti v odjemalce, ki niso brskalniki, kot je Outlook, Skype itd. V naročnini na O365 morda ni omogočena knjižnica ADAL (knjižnica preverjanja pristnosti imenika Active Directory). V tem primeru se boste morali povezati s storitvijo Exchange Online Powershell in zagnati ta ukaz »cmdlet«:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*