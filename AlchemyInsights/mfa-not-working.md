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
# <a name="issues-with-mfa"></a>Težave z MFP
So nekaj stvari v ček če uporabnik ne morem prepričevalnost using mnogo-činitelj Authentication (MFA)

1. Prizadeti uporabnik je morda blokiran v portalu Azure Active Directory. V tem primeru bodo poskusi preverjanja pristnosti za tega določenega uporabnika samodejno zavrnjeni. [Prosimo, upoštevajte navodila v tem članku, da jih odblokirate.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Če odblokiranje uporabnik didnt ' pomoč ali uporabnik ni tnalo vi moči začeti v prikrivati MFA zakaj uporabnik ter oni hoteti iti skozi vpisati proces še. [Prosimo, upoštevajte navodila v tem članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Če to je prvi čas vi usposobiti MFA ter vaš uporabnik ste nezmožen v prepričevalnost v non-browsers varovanci kot na primer razgled, Skype, etc, morda ADAL (dejanje naslovnik Authentication knjižnica) ni usposobiti naprej vaš O365 abomna. V tem primeru boste morali povezati z PowerShell Exchange Online in zaženite to cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*