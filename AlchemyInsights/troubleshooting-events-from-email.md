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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105368"
---
# <a name="troubleshooting-events-from-email"></a>Odpravljanje težav z dogodki iz e-pošte

1. Preverite, ali je funkcija omogočena za nabiralnik: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Nato si oglejte dnevnike »Dogodki iz **e-pošte« Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V dnevnikih »Dogodki iz e-pošte« poiščite IDza InternetMessageId, ki se ujema z elementom v nabiralniku.  

4. TrustScore določi, ali je element dodan ali ne. Dogodki bodo dodani le, če je TrustScore = »Zaupanja vreden«.

TrustScore določa lastnosti SPF, Dkim ali Dmarc, ki so v glavi sporočila.

Če si želite ogledati te lastnosti:

**Namizni Outlook**

- Odpiranje elementa
- File -> Properties -> Internet Headers

ali

**MFCMapi**

- Krmarjenje do elementa v mapi »Prejeto«
- Poiščite PR_TRANSPORT_MESSAGE_HEADERS_W

Te lastnosti so določene in zapisane med transportom in usmerjanjem. Za dodatno odpravljanje težav boste morda morali upoštevati podporo za prenos v zvezi z napakami v SPF, DKIM in.or DMARC.