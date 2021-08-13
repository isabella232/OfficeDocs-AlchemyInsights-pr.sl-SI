---
title: Posnetek klica 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: befb89c28396be3dc60d9d812a0c6aced69bea3c1c48d88a4ab81a34d6c259b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919007"
---
# <a name="11-call-recording"></a>Posnetek klica 1:1

Če je **gumb Začni** snemanje v klicu 1:1 zatemnjen, morate spremeniti nastavitve pravilnika za uporabnika, na kar to vpliva. Če želite preveriti nastavitev pravilnika, zaženite diagnostično diagnostiko za ega uporabnika, tako da zgoraj vnesete **Diag: Teams 1:1 Snemanje** klica zgoraj.     

Od 31. maja 2021 naprej bomo začeli vsiljevali nov pravilnik Teams za klicanje *AllowCloudRecordingForCalls.* Pred to spremembo snemanje klica v 1:1 nadzira pravilnik srečanja *AllowCloudRecording* Teams srečanja. Ta sprememba je zabeležena v objavi v središču za sporočila: [(Posodobljeno) 1:1 Uvod v pravilnik o snemanju klicev.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   Možnost pravilnika za klicanje **$False** nastavljena na privzeto nastavitev. Če želite vsem uporabnikom blokirati snemanje klicev v 1:1, vam ni treba ukrepati.  

Če želite omogočiti snemanje klicev za vse uporabnike med klici v 1:1, [uporabite Teams PowerShell,](/microsoftteams/teams-powershell-install) da zaženete ta ukaz »cmdlet«: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Lahko pa ustvarite nov pravilnik in nastavite **-AllowCloudRecordingForCalls$true** dodelite ta pravilnik uporabnikom.  

Če želite več informacij, glejte [Kontrolniki pravilnika snemanja klicev v 1:1 so (skoraj!) Tukaj](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
