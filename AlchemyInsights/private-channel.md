---
title: Zasebni kanal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005454"
---
# <a name="private-channels-in-microsoft-teams"></a>Zasebni kanali v storitvi Microsoft Teams

Zasebni kanali so nova funkcija v storitvi Microsoft teams. Upoštevajte, da zasebnih kanalov ni mogoče pretvoriti iz standardnih kanalov ali obratno.

Za podrobnosti o zasebnih kanalih, kot so informacije o [ustvarjanju zasebnega kanala in članstvu](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) ter na [zasebnih mestih SharePointovih mest](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), si oglejte [zasebne kanale v storitvi Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Opomba:** Ker konfiguracija za hranjenje zasebnih sporočil kanala še ni podprta, najemniki z omogočenimi pravilniki o hranjenju ne bodo mogli privzeto omogočiti zasebnih kanalov. Zasebne kanale lahko omogočite v skrbniškem središču ekip. Upoštevajte tudi, da je hranjenje datotek, ki so v skupni rabi v zasebnih kanalih, medtem ko hranjenje zasebnih sporočil kanala ni podprto.

**Potrebujete novega lastnika ekipe?**

Če lastnik zasebnega kanala zapusti, lahko dodate novega lastnika ekipe prek ekipe PowerShell.


- Pojdi [tukaj](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) za namestitev ekip PowerShell.

Tukaj je ukaz cmdlet boste potrebovali:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Če želite več informacij o skupini PowerShell, glejte [pregled skupin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).
