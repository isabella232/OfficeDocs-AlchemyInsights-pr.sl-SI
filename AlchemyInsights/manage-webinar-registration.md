---
title: Upravljanje registracije spletnega seminarja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794146"
---
# <a name="manage-webinar-registration"></a>Upravljanje registracije spletnega seminarja

Upravljate, kdo se lahko prijavi za Teams Webinars, tako da Teams ukazi powershell. Če želite Teams Powershell, glejte [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Privzeto je *možnost WhoCanRegister* omogočena in nastavljena na **EveryoneInCompany.** Če želite vsem, vključno z anonimnimi uporabniki, dovoliti registracijo, morate pravilnik srečanja nastaviti na **»Vsi«** z ukazom Powershell:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Opomba: Če** je v nastavitvah srečanja anonimna pridružitev izklopljena, se anonimni uporabniki ne morejo pridružiti spletnim seminarjem. Če želite izvedeti več in omogočiti to nastavitev, glejte [Upravljanje nastavitev srečanja v Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Če želite izklopiti registracijo srečanja, nastavite *AllowMeetingRegistration* na **False.**

Če želite izvedeti več o konfiguraciji, kdo se lahko prijavi za spletne seminarje, glejte [Konfiguriranje, kdo se lahko prijavi za spletne seminarje.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Če želite več informacij o nastavitvah za Microsoftove sezname, glejte [Nadzor nastavitev za Microsoftove sezname.](/sharepoint/control-lists)
