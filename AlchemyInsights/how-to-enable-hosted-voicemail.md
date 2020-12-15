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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="d8311-102">Kako omogočiti gostujočo glasovno pošto</span><span class="sxs-lookup"><span data-stu-id="d8311-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="d8311-103">Če želite omogočiti glasovno pošto, mora biti **HostedVoicemail** nastavljen na $True.</span><span class="sxs-lookup"><span data-stu-id="d8311-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="d8311-104">Lastnost **HostedVoicemail** na uporabnika z uporabo oddaljenega PowerShella (RPS).</span><span class="sxs-lookup"><span data-stu-id="d8311-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="d8311-105">Če želite več informacij o povezovanju s RPS, si oglejte [pregled Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) za več informacij o povezovanju s RPS.</span><span class="sxs-lookup"><span data-stu-id="d8311-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="d8311-106">Skrbnik za ekipe bi moral biti prijavljen v oddaljeno lupino PowerShell za ekipe.</span><span class="sxs-lookup"><span data-stu-id="d8311-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="d8311-107">V vrstici PowerShell lahko skrbnik skupine zažene **Nastavitev Set-csuser User@contoso.com-HostedVoiceMail $True** , kjer je uri SIP za uporabnika.</span><span class="sxs-lookup"><span data-stu-id="d8311-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="d8311-108">Spremembe pravilnika lahko trajajo do 24 ur, da se replicirajo.</span><span class="sxs-lookup"><span data-stu-id="d8311-108">Changes to policies can take up to 24 hours to replicate.</span></span>