---
title: Obvozna avla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684966"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Nadzor nastavitev lobija in raven sodelovanja v aplikaciji Teams

Če želite vsem, vključno s klici, zunanjimi in anonimnimi Uporabniki, omogočiti, da **zaobidejo preddverje**, uporabite PowerShell za izpolnitev tega opravila. Tukaj je primer spreminjanja globalnega pravilnika za srečanje za vašo organizacijo.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ta ukaz» cmdlet «trenutno zahteva uporabo modula za Skype za podjetja PowerShell. Če želite nastaviti nastavitev za uporabo tega ukaza» cmdlet «, si oglejte [upravljanje pravilnikov prek lupine PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Ko nastavite pravilnik, ga morate uporabiti za uporabnike; Če pa ste spremenili globalni pravilnik, bo ta samodejno veljal za uporabnike. Za vsako spremembo pravilnika morate počakati vsaj **4 ure do 24 ur** , da bodo pravilniki lahko uveljavljeni. 

Če želite, da bodo te spremembe natančno razumele, kaj to omogoča, si oglejte dokumentacijo, ki je spodaj.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumevanje kontrolnikov pravilnika lobiranja za Teams

Te nastavitve nadzirajo, kateri udeleženci srečanja čakajo v preddverju, preden so sprejeti v srečanje, in raven udeležbe, ki jim je dovoljen v srečanju. S funkcijo PowerShell lahko posodobite nastavitve pravilnika srečanja, ki še niso bile uveljavljene (z oznako» kmalu na voljo «) v skrbniškem središču za ekipe. Glejte spodaj za primer» cmdlet «lupine PowerShell, ki vsem uporabnikom omogoča, da zaobidejo preddverje.

- [Samodejno priznavanje oseb](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) je pravilnik per organizatorja, ki nadzoruje, ali se ljudje neposredno pridruževanjo srečanju ali počakajo v čakalnici, dokler jih ne sprejme uporabnik s preverjeno pristnostjo.

- [Dovolite anonimnim osebam, da začnejo srečanje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik na organizatorju, ki nadzoruje, ali se lahko anonimni ljudje, vključno z uporabniki B2B in Združenega uporabnika, pridružite srečanju uporabnikov brez preverjanja pristnosti v organizaciji.

- [Dovoli klicnim uporabnikom, da zaobidejo preddverje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kmalu**na voljo) je pravilnik na organizatorju, ki nadzoruje, ali osebe, ki kličejo s telefonom, neposredno pridružijo srečanju ali pa počakajo v preddverju, ne glede na nastavitev **samodejno priznavanje oseb** .

- [Dovoli organizatorjem, da preglasijo nastavitve lobija](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**na voljo) je pravilnik per organizatorja, ki nadzoruje, ali lahko organizator srečanja preglasi nastavitve lobija, ki jih skrbnik **samodejno prizna osebam** in **Dovoli klicne uporabnike, da zaobidejo preddverje** , ko načrtujejo novo srečanje.

**Opomba:** Preberite [upravljanje pravilnikov za srečanje v aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za srečanje Microsoft teams.
