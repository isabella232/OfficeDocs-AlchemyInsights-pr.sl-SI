---
title: Kako omogočiti gostujočo glasovno pošto
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679165"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kako omogočiti gostujočo glasovno pošto

Če želite omogočiti glasovno pošto, mora biti **HostedVoicemail** nastavljen na $True.

Lastnost **HostedVoicemail** na uporabnika z uporabo oddaljenega PowerShella (RPS).

Če želite več informacij o povezovanju s RPS, si oglejte [pregled Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) za več informacij o povezovanju s RPS.

1. Skrbnik za ekipe bi moral biti prijavljen v oddaljeno lupino PowerShell za ekipe.
1. V vrstici PowerShell lahko skrbnik skupine zažene **Nastavitev Set-csuser User@contoso.com-HostedVoiceMail $True** , kjer je uri SIP za uporabnika.

> [!NOTE]
> Spremembe pravilnika lahko trajajo do 24 ur, da se replicirajo.