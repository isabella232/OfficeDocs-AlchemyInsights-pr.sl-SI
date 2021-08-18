---
title: AggregateGroupMailbox – celotno sporočilo o neuspeli dostavi, prejeto za e-pošto, poslano Microsoft 365 skupini
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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315926"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox – celotno sporočilo o neuspeli dostavi, prejeto za e-pošto, poslano Microsoft 365 skupini

S tem ukazom ukazne lupine EXO ustvarite pravilo za prenosno Exchange za tiho spustite e-poštna sporočila, poslana v združeni nabiralnik skupine:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Opomba:** Naslov SMTP v storitvi **-SentTo zamenjajte** z naslovom SMTP nabiralnika združevalne skupine v najemniku. Iz sporočila o neuspeli dostavi lahko dobite naslov SMTP skupnega nabiralnika skupine.



