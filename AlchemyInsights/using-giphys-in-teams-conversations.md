---
title: Uporaba Giphy v pogovorih Teams
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982577"
---
# <a name="using-giphys-in-teams-conversations"></a>Uporaba Giphy v pogovorih Teams

Giphy Access v programu Teams chat je privzeto omogočen. Kot skrbnik lahko nadzorujete, ali so Giphy na voljo uporabnikom tako, da [nastavite pravilnik za sporočanje](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) in zagotovite, da je **Uporaba giphy v pogovorih** **vklopljena**.

Če gif v pogovorih Teams ne deluje po pričakovanjih, preverite:

[Pravilnik za sporočanje](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora omogočiti giphy. Če želite preveriti z uporabo ukazov» cmdlet «PowerShell:

- Preverite, ali lahko [upravljate ekipe z lupino PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Zaženite ukaz PowerShell [Get-CsTeamsMessagingPolicy-Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) in preverite, ali je **AllowGiphy** nastavljena na **True**.
- Če je argument» **AllowGiphy** «nastavljen na» **FALSE «** , zaženite ta ukaz» [set-CsTeamsMessagingPolicy – Identity «(globalno AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Če želite omogočiti dostop do URL-ja» Giphy «, morate omogočiti [izbirne povezave](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Če imate več pravilnikov za sporočanje Teams, konfiguriranih za najemnika, lahko določite identiteto pravilnika, dodeljenega uporabniku, ki je bil uporabnik, z ukazom PowerShell [Get-CsOnlineUser – Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Izberite TeamsMessagingPolicy.
