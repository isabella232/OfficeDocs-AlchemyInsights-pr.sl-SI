---
title: Nastavitve pravilnika srečanja
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704622"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilnikov za srečanje v aplikaciji Microsoft Teams

**Opomba: Če želite, da bodo spremembe pravilnika veljale za uporabnike, lahko traja do 24 ur.** Morda ne boste mogli takoj spreminjati novih pravilnikov; Počakajte 4 ure in poskusite znova spremeniti novo ustvarjen pravilnik.

Pravilniki o srečanju se uporabljajo za nadzor funkcij, ki so na voljo za srečanja udeležencev za srečanja, ki jih načrtujejo uporabniki v vaši organizaciji. Nekatere funkcije pravilnikov srečanja morda ne bodo uveljavljene v skrbniškem središču za Teams (ti so označeni» kmalu na voljo «v dokumentaciji). V tem primeru ali če se prikaže sporočilo o napaki, kot je» trenutno ne moremo posodobiti pravilnika, vendar poskusite znova pozneje «v skrbniškem središču za Microsoft Teams, vam priporočamo, da uporabite PowerShell za ustvarjanje ali spreminjanje pravilnikov skupine za srečanje. 

Če želite več informacij o pravilnikih za srečanje, si oglejte te vire:

- Če želite izvedeti več o ustvarjanju pravilnikov, spreminjanju in dodeljevanju uporabnikov v pravilnik, glejte [upravljanje pravilnikov za srečanje v aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Če želite spremeniti pravilnike z ukazi» cmdlet «PowerShell, glejte [pregled skupine PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Za pravilnike o srečanju Teams morate uporabiti [modul za Skype za podjetja PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) . 
    - Če želite več informacij, si oglejte [dokumentacijo» cmdlet «za CsTeamsMeetingPolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

