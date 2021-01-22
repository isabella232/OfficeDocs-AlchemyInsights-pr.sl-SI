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
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935139"
---
# <a name="turn-on-ndi-technology"></a>Vklop tehnologije NDI

Tehnologija NDI zahteva, da je za uporabnika vklopljena dva koraka:

1. Skrbnik najemnika mora omogočiti lastnost» AllowNDIStreaming «v CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Ko je ta sprememba izpolnjena, mora končni uporabnik vklopiti NDI® tehnologijo za določenega odjemalca iz **nastavitev > dovoljenja**.

Če želite več informacij, glejte [Uporaba tehnologije NDI v aplikaciji Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
