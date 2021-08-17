---
title: Obhodna čakalnica
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
- "2673"
- "9000740"
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059612"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Nadziranje nastavitev čakalnice in raven sodelovanja v Teams

Če želite vsem, vključno s klicnimi, zunanjimi in anonimnimi uporabniki, dovoliti, da preskočijo čakalnico **,** za dokončanje tega opravila uporabite PowerShell. Spodaj je primer spreminjanja pravilnika globalnega srečanja za vašo organizacijo.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ta ukaz »cmdlet« trenutno zahteva uporabo Skype za podjetja PowerShell. Če želite nastaviti uporabo tega ukaza »cmdlet« , si oglejte [Upravljanje pravilnikov prek lupine PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Ko nastavite pravilnik, ga morate uporabiti za uporabnike. če ste spremenili globalni pravilnik, pa bo samodejno veljal za uporabnike. Če želite spremeniti pravilnik, morate počakati vsaj 4 ure do **24** ur, da bodo pravilniki veljati. 

Preden spremenite dokument, preberite spodnjo dokumentacijo, da boste natančno razumeli, kaj to omogoča.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumevanje Teams pravilnika čakalnice srečanja

Te nastavitve nadzirajo, kateri udeleženci srečanja počakajo v čakalnici, preden so sprejeti v srečanje, in raven sodelovanja, ki jim je dovoljena v srečanju. S storitvijo PowerShell lahko posodobite nastavitve pravilnika srečanja, ki še niso bile implementirane (v skrbniškem središču za Office Teams kmalu na voljo). Glejte spodaj za primer ukaza »cmdlet« lupine PowerShell, ki vsem uporabnikom omogoča, da preskočijo čakalnico.

- [Samodejno sprejem oseb je](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) pravilnik na organizatorja, ki nadzira, ali se osebe pridružijo srečanju neposredno ali pa počakajo v čakalnici, dokler jih ne sprejmejo uporabnik s preverjeno pristnostjo.

- [Anonimnim](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) ljudem dovoli začetek srečanja je pravilnik na organizatorja, ki nadzira, ali se lahko anonimne osebe, vključno z B2B in zunanji uporabniki, pridružijo srečanju uporabnika brez preverjenega uporabnika iz organizacije, ki se udeleži.

- [Dovoli,](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) da klicni uporabniki preskočijo čakalnico **(** kmalu na voljo ) je pravilnik na organizatorja, ki nadzira, ali se osebe, ki so se srečanju neposredno pridružile s klicem po telefonu, ali pa počakajo v čakalnici ne glede na nastavitev Samodejno dovoli **dostop** oseb.

- [Dovoli](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) organizatorjem, da preglasijo nastavitve čakalnice **(** kmalu na voljo ) je pravilnik na  organizatorja, ki nadzoruje, ali lahko organizator srečanja preglasi nastavitve čakalnice, ki jih je nastavil skrbnik v možnosti Samodejno dovoli sprejem oseb **in** Dovoli, da klicni uporabniki preskočijo čakalnico, ko načrtujejo novo srečanje.

**Opomba:** Če [želite popoln pregled Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) srečanja, preberite Upravljanje pravilnikov Microsoft Teams srečanja.
