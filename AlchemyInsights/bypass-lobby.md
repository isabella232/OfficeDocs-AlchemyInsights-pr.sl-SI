---
title: Obvoznica v preddverju
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376837"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Nadzor nastavitev lobistov in raven udeležbe

Te nastavitve nadzorujejo, kateri Udeleženci sestanka čakajo v preddverju, preden so sprejeti na sestanek, in raven udeležbe, ki so jim dovoljene na sestanku. Z lupino PowerShell lahko posodobite nastavitve pravilnika za sestanke, ki še niso bile izvedene (z oznako» kmalu «) v skrbniškem središču ekip.  Glej spodaj za primer cmdlet PowerShell, ki omogoča vsem uporabnikom, da zaobide lobby.  

- [Samodejno priznam](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , da so ljudje po-organizator politike, ki nadzoruje, ali se ljudje pridružijo srečanju neposredno ali čakati v preddverju, dokler jih ne sprejme overjeni uporabnik.

- [Omogočanje anonimnih oseb, da začnejo sestanek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik za organizatorja, ki nadzoruje, ali se lahko anonimni ljudje, vključno z B2B in federativne Uporabniki, pridružijo sestanku uporabnika brez overjenega uporabnika iz organizacije v navzočnosti.

- [Omogučiti sončna ura-v uporabnik v bypass preddverje](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**bodoč zgodaj**) je a po-organizator zvitost to kontrolni aparati ali narod kdo sončna ura v z telefon združiti sestanek naravnost ali čakati v preddverje če ne **automatically priznajte narod** postavljanje.

- [Dovolite organizatorjem, da preglasijo nastavitve v preddverju](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**) je pravilnik za organizatorja, ki nadzira, ali lahko organizator srečanja preglasi nastavitve v preddverju, ki jih admin Nastavi v **samodejno prizna ljudi** in **Dovoli klicanje uporabnikom, da obidejo preddverje** , ko načrtujete nov sestanek.

**Opomba:** Preberite [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za sestanke programa Microsoft teams. 


**Primer lupine**

Če želite vsem, vključno z zunanjimi ali anonimnimi Uporabniki, dovoliti, da zaobide čakalnico, lahko za dokončanje te naloge uporabite tudi lupino PowerShell.  Tukaj je primer spreminjanja globalne politike srečanja za vašo organizacijo.   

(Bodite prepričani, da pregleda dokumentacijo zgoraj, preden te spremembe razumeti, kaj to omogoča.)

Set-CsTeamsMeetingPolicy-identiteta Global-Autovključitvi Tedusers "vsakdo"-AllowPSTNUsersToBypassLobby $True

Če želite več informacij, glejte [set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).
