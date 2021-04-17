---
title: Nastavitve pravilnika srečanja
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825459"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilnikov za srečanja v aplikaciji Microsoft Teams

**Opomba: Traja lahko do 24 ur, preden spremembe pravilnika začne veljati za uporabnike.** Morda ne boste mogli takoj spreminjati novo ustvarjenih pravilnikov; počakajte 4 ure in poskusite znova spremeniti novo ustvarjeni pravilnik.

S pravilniki srečanja nadzorujete funkcije, ki so na voljo udeležencem srečanja za srečanja, ki jih načrtujejo uporabniki v organizaciji. Nekatere funkcije pravilnikov srečanja morda še ne bodo na voljo v skrbniškem središču za Teams (v dokumentaciji so označene kot »kmalu na voljo«). Če se v tem primeru prikaže napaka, kot je »Pravilnika trenutno ni mogoče posodobiti, lahko pa ga poskusite znova pozneje« v skrbniškem središču za Microsoft Teams, priporočamo, da uporabite PowerShell za ustvarjanje ali spreminjanje pravilnikov za srečanja v storitvi Teams. 

Če želite več informacij o pravilnikih srečanja, glejte te vire:

- Če želite izvedeti več o ustvarjanju pravilnikov, spremembami in dodeljevanju uporabnikov pravilniku, glejte [Upravljanje pravilnikov o srečanju v teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Če želite spremeniti pravilnik z ukazi »cmdlet« lupine PowerShell, glejte [Pregled storitve PowerShell za Teams.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Uporabiti morate modul [PowerShell za Skype za podjetja za pravilnike](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) srečanja v storitvi Teams. 
    - Za več informacij preglejte dokumentacijo z ukazi [»cmdlet« *-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)

