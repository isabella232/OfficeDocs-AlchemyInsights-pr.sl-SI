---
title: AggregateGroupMailbox – celotno sporočilo o neuspeli dostavi, prejeto po e-pošti, Microsoft 365 skupini
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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951869"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox – celotno sporočilo o neuspeli dostavi, prejeto po e-pošti, Microsoft 365 skupini

Uporabite ta ukazne lupine EXO, če želite ustvariti prenosno pravilo za Exchange za tiho spustite e-poštna sporočila, poslana v združeni nabiralnik skupine:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Naslov SMTP v storitvi **-SentTo zamenjajte** z naslovom SMTP nabiralnika združevalne skupine v najemniku. Iz sporočila o neuspeli dostavi lahko dobite naslov SMTP skupnega nabiralnika skupine.



