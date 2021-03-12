---
title: snemanje klicev v 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733865"
---
# <a name="11-call-recording"></a>snemanje klicev v 1:1

Skrbniki morajo zdaj ukrepati, da bodo lahko uporabniki beležili 1:1 klicev.
 
Začetek april 12, 2021, bomo začeli uveljaviti novo Teams Calling Policy option *AllowCloudRecordingForCalls*. 

Trenutno so zmogljivosti snemanja klicev v 1:1 nadzorovane z možnostjo *AllowCloudRecording* v pravilnikih za srečanje ekip. Če lahko vaši uporabniki snemajo sestanke v Teams, bodo morda snemali tudi 1:1 klicev.

Če želite blokirati vse uporabnike iz snemanja 1:1 klicev, vam ni treba izvesti nobenega dejanja. Možnost» *AllowCloudRecordingForCalls* Calling pravilnik «bo privzeto $FALSE.

Ta sprememba je dokumentirana v tej objavi v središču za sporočila: [(posodobljeno) 1:1 vnos pravilnika o snemanju](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) , da nastavite možnost pravilnika za [klicanje ekip](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Če želite omogočiti snemanje klicev v 1:1 klici:** Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $True

**Če želite onemogočiti snemanje klicev v 1:1 klici:** Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $FALSE

