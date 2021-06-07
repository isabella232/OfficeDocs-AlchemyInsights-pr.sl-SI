---
title: Omogočanje Teams Webinars
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794039"
---
# <a name="enable-teams-webinars"></a>Omogočanje Teams Webinars

Spletni seminarji so omogočeni privzeto. Upravljate lahko, kdo lahko načrtuje in registrira za Teams webinars, tako da Teams ukazi powershell.

- Vsi uporabniki, ki lahko ustvarijo srečanje, lahko prav tako ustvarijo srečanje spletnega seminarja. Če želite upravljati, kdo lahko načrtuje Teams Webinars, uporabite *AllowMeetingRegistration.* 
- Privzeto je *možnost WhoCanRegister* omogočena in nastavljena na **Vsi.** Če želite izklopiti registracijo srečanja, nastavite *AllowMeetingRegistration* na **False.**

Če želite spremeniti te nastavitve, morate namestiti [Teams PowerShell.](/microsoftteams/teams-powershell-install) Pravilniki srečanja se izvajajo tudi za spletne Teams spletnih seminarjih. Če je na primer anonimna pridružitev v nastavitvah srečanja izklopljena, se anonimni uporabniki ne morejo pridružiti spletnim seminarjem.

Če želite izvedeti več o konfiguraciji, kdo se lahko prijavi za spletne seminarje, glejte [Konfiguriranje, kdo se lahko prijavi za spletne seminarje.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Če želite več informacij o nastavitvah za Microsoftove sezname, glejte [Nadzor nastavitev za Microsoftove sezname.](/sharepoint/control-lists)