---
title: Uporaba giphy v Teams pogovorih
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104324"
---
# <a name="using-giphys-in-teams-conversations"></a>Uporaba giphy v Teams pogovorih

Dostop s giphy Teams klepetu je privzeto omogočen. Kot skrbnik lahko nadzorujete, ali so Giphy [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) na voljo za uporabnike, tako da nastavite pravilnik sporočanja in zagotovite, da je nastavitev **»Uporabi Giphy v pogovorih«** **»On«**(Uporabljaj Giphy v pogovorih) .

Če GIF-i v pogovorih ne delujejo po pričakovanjih Teams, preverite:

Pravilnik [sporočanja](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora omogočiti Giphy. Preverjanje z ukazi »cmdlet« lupine PowerShell:

- Preverite, ali lahko [upravljate Teams z lupino PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Zaženite ukaz PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) in preverite, ali je **allowGiphy** nastavljena na **TRUE.**
- Če **je allowGiphy** nastavljena na **FALSE,** zaženite ta ukaz PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Izbirne povezane izkušnje](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) morajo biti omogočene, če želite omogočiti dostop do URL-ja Giphy.

> [!NOTE]
> Če imate za najemnika konfiguriranih več pravilnikov sporočanja v storitvi Teams, lahko določite identiteto pravilnika, ki je dodeljen vplivu, z ukazom PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Izberite TeamsMessagingPolicy.
