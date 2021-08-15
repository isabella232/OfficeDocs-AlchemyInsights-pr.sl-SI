---
title: Vklop tehnologije NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023538"
---
# <a name="turn-on-ndi-technology"></a>Vklop tehnologije NDI

Tehnologija NDI za uporabnika zahteva dva koraka:

1. Skrbnik najemnika mora omogočiti lastnost »AllowNDIStreaming« v CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Ko je ta sprememba izpolnjena, mora končni uporabnik vklopiti tehnologijo NDI® za določenega odjemalca iz **Nastavitve > dovoljenja.**

Če želite več informacij, [glejte Uporaba tehnologije NDI v Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
