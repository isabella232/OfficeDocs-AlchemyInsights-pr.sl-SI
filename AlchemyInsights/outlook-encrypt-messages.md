---
title: S/MIME v programu Outlook v spletu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772314"
---
# <a name="encrypt-email-messages-in-outlook"></a>Šifriranje e-poštnih sporočil v Outlooku

Šifriranje sporočil v storitvi Microsoft 365 je zgrajeno na Microsoft Azure Rights Management (Azure RMS), ki je del zaščite informacij Azure. Če vaša naročnina vključuje upravljanje pravic v storitvi Azure ali Azure, **vam ni treba izvesti nobenih dejanj, s katerimi lahko ročno omogočite ali aktivirate** storitev za upravljanje pravic.

Na podlagi povratnih informacij strank vam ne bomo več omogočili pravil pretoka pošte Exchange za samodejno šifriranje odhodnih e-poštnih sporočil, ki vsebujejo določeno vrsto občutljivih informacij v najemniku. Namesto tega zagotavljamo podrobna navodila o tem, kako lahko to naredite sami. Če želite več podrobnosti o tem, kako ustvarite pravilo prenosa za šifriranje občutljivih informacij, si oglejte [Ta članek](https://aka.ms/OmeEtr).

- Če uporabljate Outlook v spletu (prej **OWA**): pri sestavljanju e-poštnega sporočila preprosto kliknite **zaščiti** v programu owa. S tem boste uporabili dovoljenje» ne Posreduj «. Kliknite **Spremeni dovoljenje** in izberite **Šifriraj** , da le šifrirate sporočilo.

- Če uporabljate **Outlook Client**: Če želite poslati šifrirano sporočilo iz Outlooka 2013 ali 2016 ali Outlook 2016 za Mac, izberite **možnosti**  >  **dovoljenja**, nato pa izberite možnost zaščite, ki jo potrebujete.

- Če želite **samodejno šifrirati vso e-pošto** , poslano nekaterim prejemnikom ali zunanjim partnerjem, morate ustvariti pravilo prenosa pošte v skrbniškem središču za Exchange. Podrobna navodila so na voljo v [tem članku podpore](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

