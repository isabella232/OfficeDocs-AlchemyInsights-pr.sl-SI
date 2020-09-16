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
# <a name="issues-with-azure-mfa"></a>Težave s storitvijo Azure MFA
Če želite preveriti, ali se uporabniki ne morejo prijaviti z uporabo multi-Factor Authentication (MFA), lahko preverite nekaj stvari

1. Prizadeti uporabnik je lahko blokiran v portalu Azure Active Directory. Če je to res, bodo poskusi preverjanja pristnosti tega določenega uporabnika samodejno zavrnjeni. [Upoštevajte navodila v tem članku, da jih odblokirate.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Če deblokiranje uporabnika ni pomagalo ali uporabnik ni blokiran, lahko poskusite ponastaviti MFA za uporabnika in bodo znova vzpostavili postopek za včlanitev. [Upoštevajte navodila v tem članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Če je to prvič, da ste omogočili MFA in se vaši uporabniki ne morejo prijaviti v odjemalce, ki niso brskalniki, kot so Outlook, Skype itd., morda knjižnice ADAL (knjižnica za preverjanje pristnosti imenika Active Directory) ni omogočena v naročnini na O365. V tem primeru se boste morali povezati s storitvijo Exchange Online PowerShell in zagnati ukaz» cmdlet «:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*