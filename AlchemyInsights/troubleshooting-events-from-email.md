---
title: Odpravljanje težav z dogodki iz e-pošte
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834855"
---
# <a name="troubleshooting-events-from-email"></a>Odpravljanje težav z dogodki iz e-pošte

1. Preverite, ali je funkcija omogočena za nabiralnik: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Nato si oglejte dnevnike »Dogodki iz **e-pošte« Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V dnevnikih »Dogodki iz e-pošte« poiščite IDza InternetMessageId, ki se ujema z elementom v nabiralniku.  

4. TrustScore določi, ali je element dodan ali ne. Dogodki bodo dodani le, če je TrustScore = »Zaupanja vreden«.

TrustScore določa lastnosti SPF, Dkim ali Dmarc, ki so v glavi sporočila.

Če si želite ogledati te lastnosti:

**Namizna različica Outlooka**

- Odpiranje elementa
- File -> Properties -> Internet Headers

ali

**MFCMapi**

- Krmarjenje do elementa v mapi »Prejeto«
- Poiščite PR_TRANSPORT_MESSAGE_HEADERS_W

Te lastnosti so določene in zapisane med transportom in usmerjanjem. Za dodatno odpravljanje težav boste morda morali upoštevati podporo za prenos v zvezi z napakami v SPF, DKIM in.or DMARC.