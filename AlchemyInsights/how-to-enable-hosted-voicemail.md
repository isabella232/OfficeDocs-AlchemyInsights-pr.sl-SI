---
title: Kako omogočiti gostovano glasovno pošto
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318664"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kako omogočiti gostovano glasovno pošto

Če želite omogočiti glasovno pošto, mora biti možnost **HostedVoicemail** $true.

Lastnost **HostedVoicemail za** uporabnika, ki uporablja Remote PowerShell (RPS).

Če želite več informacij o povezovanju s RPS, [glejte Microsoft Teams Pregled lupine PowerShell,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) če želite več informacij o povezovanju s RPS.

1. Skrbnik Teams mora biti prijavljeni v oddaljeno sejo PowerShell, da Teams.
1. Iz lupine PowerShell Teams Skrbnik lahko zažene **set-csuser user@contoso.com -HostedVoiceMail $true** kjer je sip uri zadevni uporabnik.

**Opomba:** Pri spremembah pravilnikov lahko traja do 24 ur, da se pravilniki podvojijo.