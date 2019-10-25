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
ms.openlocfilehash: 6632bb0c09c7ce99f14cd55582025b37a846369d
ms.sourcegitcommit: ee719f011f766fc20d23e935e98d7e33c326183b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/24/2019
ms.locfileid: "37654272"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Nadzor nastavitev lobistov in raven udeležbe

Če želite dovoliti vsem, vključno z dial-in, zunanjimi in anonimnimi Uporabniki, da zaobide preddverje, lahko uporabite PowerShell za to. Tukaj je primer spreminjanja globalne politike srečanja za vašo organizacijo:

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ta ukaz» cmdlet «trenutno zahteva uporabo modula Skype za podjetja PowerShell. Če želite dobiti nastavitev za uporabo tega ukaza» cmdlet «, si oglejte [pravilnike upravljanja prek lupine PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Nastavite lahko novo politiko, ki jo boste nato morali uporabiti za uporabnike. Če spremenite globalno politiko, bo samodejno veljala za uporabnike. Za vsako spremembo pravilnika morate počakati vsaj 4 ure in do 24 ur, da se bodo pravilniki uveljavili.

Bodite prepričani, da pregleda dokumentacijo spodaj, preden te spremembe razumeti, kaj to omogoča.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumevanje ekip, ki izpolnjujejo nadzorne politike lobistov

- [Samodejno priznam](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , da so ljudje po-organizator politike, ki nadzoruje, ali se ljudje pridružijo srečanju neposredno ali čakati v preddverju, dokler jih ne sprejme overjeni uporabnik.

- [Omogočanje anonimnih oseb, da začnejo sestanek](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik za organizatorja, ki nadzoruje, ali se lahko anonimni ljudje, vključno z B2B in federativne Uporabniki, pridružijo sestanku uporabnika brez overjenega uporabnika iz organizacije v navzočnosti.

- [Omogučiti sončna ura-v uporabnik v bypass preddverje](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**bodoč zgodaj**) je a po-organizator zvitost to kontrolni aparati ali narod kdo sončna ura v z telefon združiti sestanek naravnost ali čakati v preddverje če ne **automatically priznajte narod** postavljanje.

- [Dovolite organizatorjem, da preglasijo nastavitve v preddverju](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**) je pravilnik za organizatorja, ki nadzira, ali lahko organizator srečanja preglasi nastavitve v preddverju, ki jih admin Nastavi v **samodejno prizna ljudi** in **Dovoli klicanje uporabnikom, da obidejo preddverje** , ko načrtujete nov sestanek.

**Opomba:** Preberite [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za sestanke programa Microsoft teams.
