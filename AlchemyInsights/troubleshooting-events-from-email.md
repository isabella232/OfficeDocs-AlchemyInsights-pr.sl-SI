---
title: Odpravljanje težav z e-pošto
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658750"
---
# <a name="troubleshooting-events-from-email"></a>Odpravljanje težav z e-pošto

1. Preverite, ali je funkcija omogočena za nabiralnik: **Get-EventsFromEmailConfiguration- <mailbox> Identity**

2. Nato si oglejte dnevniki» dogodki iz e-pošte « **Izvozi – MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. V dnevnikih» dogodki iz e-pošte «poiščite InternetMessageId, ki se ujema z elementom v nabiralniku.  

4. TrustScore določi, ali je element dodan ali ne. Dogodki bodo dodani le, če je TrustScore = "zaupanja vreden".

TrustScore je določen z lastnostmi SPF, DKIM ali dMarc, ki so v glavi sporočila.

Če si želite ogledati te lastnosti:

**Namizni Outlook**

- Odpiranje elementa
- Lastnosti datoteke >-> internetne glave

ali

**MFCMapi**

- Pomikanje do elementa v mapi» Prejeto «
- Poiščite PR_TRANSPORT_MESSAGE_HEADERS_W

Te lastnosti so določene in zabeležene med prevozom in usmerjanjem. Če želite dodatno odpraviti težave, boste morda morali nadaljevati s podporo za prenos informacij o napakah v SPF, DKIM in. or DMARC.