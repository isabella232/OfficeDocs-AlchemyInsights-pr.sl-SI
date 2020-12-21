---
title: AggregateGroupMailbox Full NDR, ki ste ga prejeli za e-pošto, poslano v skupino Microsoft 365
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
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722079"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox Full NDR, ki ste ga prejeli za e-pošto, poslano v skupino Microsoft 365

Z ukazom EKSO Shell lahko ustvarite pravilo za prenos prenosa za tiho spuščanje e-poštnih sporočil, poslanih v združevalni nabiralnik skupine:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Zamenjajte naslov SMTP v storitvi **SentTo** z naslovom SMTP za Združeno skupino nabiralnika v najemniku. Naslov SMTP Združenega skupinskega nabiralnika lahko pridobite iz prejetega poročila NDR.



