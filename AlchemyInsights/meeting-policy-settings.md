---
title: Nastavitve pravilnika za sestanke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376832"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Upravljanje pravilnikov za sestanke v storitvi Microsoft Teams

Pravilniki za sestanke se uporabljajo za nadzor funkcij, ki so na voljo za srečanje udeležencev za sestanke, ki so jih načrtovali uporabniki v vaši organizaciji. Nekaterih funkcij pravilnikov za sestanke morda ne boste izvajali v skrbniškem središču ekip (ti so označeni z "kmalu" v dokumentaciji). V tem primeru ali če dobivate napako, kot je» trenutno ne moremo posodobiti pravilnika, ampak poskusite znova pozneje «v skrbniškem središču za Microsoft Teams priporočamo, da uporabite lupino PowerShell za ustvarjanje ali spreminjanje pravilnikov sestankov skupine. 

Če želite več informacij o politikah za sestanke, si oglejte te vire:

- Če želite izvedeti več o ustvarjanju pravilnikov, spreminjanju in dodeljevanju uporabnikov pravilniku, glejte [upravljanje pravilnikov za sestanke v storitvi Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).

- Če želite spremeniti pravilnik s pomočjo ukazov» cmdlet «PowerShell, glejte [pregled skupin PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Za pravilnike za sestanke ekip morate uporabiti [modul Skype za podjetja PowerShell](https://www.microsoft.com/download/details.aspx?id=39366) . 
    - Preglejte [dokumentacijo» cmdlet «*-csteamsmeetingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) za več informacij.

**Opomba:** Do 24 ur lahko traja, da spremembe pravilnika uveljavljajo za uporabnike. Na novo ustvarjene pravilnike morda ne boste mogli takoj spreminjati; Počakajte 4 ure in znova poskusite spremeniti novo ustvarjeno politiko. Če imate še vedno težave, poskusite PowerShell.  