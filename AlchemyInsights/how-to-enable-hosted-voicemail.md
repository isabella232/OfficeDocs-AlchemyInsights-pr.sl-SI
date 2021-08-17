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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055570"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kako omogočiti gostovano glasovno pošto

Če želite omogočiti glasovno pošto, mora biti možnost **HostedVoicemail** $true.

Lastnost **HostedVoicemail za** uporabnika, ki uporablja Remote PowerShell (RPS).

Če želite več informacij o povezovanju s RPS, [glejte Microsoft Teams pregled lupine PowerShell,](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) če želite več informacij o povezovanju s RPS.

1. Skrbnik Teams mora biti prijavljeni v oddaljeno sejo PowerShell za Teams.
1. Iz lupine PowerShell Teams Skrbnik lahko zažene **set-csuser user@contoso.com -HostedVoiceMail $true** kjer je sip uri zadevni uporabnik.

> [!NOTE]
> Spremembe pravilnikov lahko trajajo do 24 ur, da se pravilniki podvojijo.