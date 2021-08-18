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
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323536"
---
# <a name="using-giphys-in-teams-conversations"></a>Uporaba giphy v Teams pogovorih

Dostop s giphy Teams klepetu je privzeto omogočen. Kot skrbnik lahko nadzorujete, ali so Giphy [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) na voljo uporabnikom, tako da nastavite pravilnik sporočanja in zagotovite, da je nastavitev **»Uporabi Giphy v pogovorih«** **»On«**(Uporabljaj Giphy v pogovorih) .

Če GIF-i v pogovorih ne Teams v skladu s pričakovanji, preverite:

Pravilnik [sporočanja](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora omogočiti Giphy. Preverjanje z ukazi »cmdlet« lupine PowerShell:

- Preverite, ali lahko [upravljate Teams z lupino PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Zaženite ukaz PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) in preverite, ali je **allowGiphy** nastavljena na **TRUE.**
- Če **je allowGiphy** nastavljena na **FALSE,** zaženite ta ukaz PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Izbirne povezane izkušnje](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) morajo biti omogočene, če želite omogočiti dostop do URL-ja Giphy.

**Opomba:** Če imate za najemnika konfiguriranih več pravilnikov za sporočanje v storitvi Teams, lahko določite identiteto pravilnika, ki je dodeljen vplivu, z ukazom PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Izberite TeamsMessagingPolicy.
