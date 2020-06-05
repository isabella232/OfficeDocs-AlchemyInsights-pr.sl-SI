---
title: Odpravljanje težav pri dogodkih iz e-pošte
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569403"
---
# <a name="troubleshooting-events-from-email"></a>Odpravljanje težav pri dogodkih iz e-pošte

1. Preverite, ali je funkcija omogočena za nabiralnik: **zaslužiti-EventsFromEmailConfiguration-identiteta <mailbox> **

2. Potem poglej "dogodki iz e-pošte" dnevniki **Export-Mailboxdiagnosticdnevniki <mailbox> -Component timeprofile**

3. V dnevnikih» dogodki iz e-pošte «poiščite InternetMessageId, ki se ujema z elementom v nabiralniku.  

4. Vrednost TrustScore določa, ali je artikel dodan ali ne. Dogodki bodo dodani le, če je TrustScore = "zaupanja vreden".

TrustScore določa lastnosti SPF, DKIM ali dMarc, ki so v glavi sporočila.

Če si želite ogledati te lastnosti:

**Namizni obeti**

- Odpiranje elementa
- Datoteke-lastnosti >-> internetne glave

Ali

**MFCMapi**

- Pomikanje do elementa v mapi» Prejeto «
- Poiščite PR_TRANSPORT_MESSAGE_HEADERS_W

Te lastnosti se določijo in zabeležijo med transportom in usmerjanjem. Za nadaljnje odpravljanje težav boste morda morali spremljati prometno podporo o napakah v SPF, DKIM in. ali DMARC.