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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250181"
---
# <a name="issues-with-mfa"></a>Vprašanja z MZZ
Obstaja nekaj stvari, da preverite, če uporabnikov ne morete prijaviti z uporabo multi-overjanja (MFP)

1. Uporabnikov lahko blokiran v Azure Active Directory Portal. Če je temu tako, preverjanje pristnosti poskusov za to določenega uporabnika bo samodejno zavrnjen. [Prosimo, sledite korakom v tem članku, da jih odblokirate.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Če deblokiranje uporabnik ni pomagalo ali uporabnik ni tnalo vi moči začeti vprikrivati MFP za uporabnika in bo šel skozi proces enroll spet. [Prosimo, sledite korakom v tem članku.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Če je prvič omogočena MZZ in uporabniki ste nezmožen v prepričevalnost-brskalniki stranke, kot so Outlook, Skype, itd, morda ADAL (Active Directory preverjanje pristnosti knjižnico) ni omogočen na naročnino O365. V tem primeru boste morali povezati Exchange Online Powershell in zaženite ukaz cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*