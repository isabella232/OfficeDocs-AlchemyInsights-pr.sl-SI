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
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889098"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Nadzor nastavitev lobistov in raven udeležbe v ekipah

Če želite omogočiti vsem, vključno z dial-in, zunanjimi in anonimnimi Uporabniki, da **zaobide preddverje**, uporabite PowerShell za dokončanje te naloge. Tukaj je primer spreminjanja globalne politike srečanja za vašo organizacijo.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ta ukaz» cmdlet «trenutno zahteva uporabo modula Skype za podjetja PowerShell. Če želite nastaviti uporabo tega ukaza» cmdlet «, preverite [pravilnike upravljanja prek lupine PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Ko nastavite pravilnik, ga morate uporabiti za uporabnike; ali, če ste spremenili globalno politiko, se bo samodejno uporabljal za uporabnike. Za vsako spremembo pravilnika morate počakati vsaj **4 ure do 24 ur** , da se bodo pravilniki uveljavili. 

Bodite prepričani, da pregleda dokumentacijo spodaj, preden te spremembe razumeti, kaj to omogoča.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumevanje ekip, ki izpolnjujejo nadzorne politike lobistov

Te nastavitve nadzorujejo, kateri Udeleženci sestanka čakajo v preddverju, preden so sprejeti na sestanek, in raven udeležbe, ki so jim dovoljene na sestanku. Z lupino PowerShell lahko posodobite nastavitve pravilnika za sestanke, ki še niso bile izvedene (z oznako» kmalu «) v skrbniškem središču ekip. Glej spodaj za primer cmdlet PowerShell, ki omogoča vsem uporabnikom, da zaobide lobby.

- [Samodejno priznam](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , da so ljudje po-organizator politike, ki nadzoruje, ali se ljudje pridružijo srečanju neposredno ali čakati v preddverju, dokler jih ne sprejme overjeni uporabnik.

- [Omogočanje anonimnih oseb, da začnejo sestanek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik za organizatorja, ki nadzoruje, ali se lahko anonimni ljudje, vključno z B2B in federativne Uporabniki, pridružijo sestanku uporabnika brez overjenega uporabnika iz organizacije v navzočnosti.

- [Omogučiti sončna ura-v uporabnik v bypass preddverje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**bodoč zgodaj**) je a po-organizator zvitost to kontrolni aparati ali narod kdo sončna ura v z telefon združiti sestanek naravnost ali čakati v preddverje če ne **automatically priznajte narod** postavljanje.

- [Dovolite organizatorjem, da preglasijo nastavitve lobistov](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**) je pravilnik za organizatorja, ki nadzira, ali lahko organizator srečanja preglasi nastavitve v preddverju, ki jih skrbnik Nastavi v **samodejno Sprejmi ljudi** in **Dovoli uporabnikom klicanja, da obidejo čakalnico** , ko razporeja novo sejo.

**Opomba:** Preberite [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za sestanke programa Microsoft teams.
