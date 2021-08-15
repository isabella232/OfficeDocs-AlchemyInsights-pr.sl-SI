---
title: Diagnostika za težave z dostopom do različnih vrat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030918"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostika za težave z dostopom do različnih vrat

Če želite odpraviti različne težave z dostopom do vrat, izvedite te korake:

1. Ustavite/prestavite navidezni računalnik (VM) iz portala, znova zaženite navidezni računalnik in ga znova preskusite. 
2. Preverite omrežne nastavitve svojega načla, da ugotovite, ali vaš promet blokirajo omrežne varnostne skupine (NSG). Uporabite lahko tudi orodje za preverjanje toka IP storitve [Network Watcher,](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) da preverite, ali NSG-ji, ki blokirajo promet, poti User-Defined (UDR) preusmerijo promet nazaj na mestu uporabe ('Privzeta pot' 0.0.0.0/0) ali na omrežno napravo.
Če po zgornjih korakih še vedno pride do težav, navedite ime naVM in vrata TCP, na katere poskušate poslati e-pošto, da bodo nadaljnja navodila.

**Priporočeni dokumenti**

[Omejitve in priporočila za pošiljanje odhodne e-pošte prek vrat 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)