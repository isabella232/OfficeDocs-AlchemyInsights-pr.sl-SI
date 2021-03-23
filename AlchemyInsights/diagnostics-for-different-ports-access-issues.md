---
title: Diagnostika za različne težave z dostopom do vrat
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
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036808"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostika za različne težave z dostopom do vrat

Če želite odpraviti različne težave z dostopom do vrat, izvedite te korake:

1. Ustavite/odrazdelite navidezni stroj (VM) iz portala, znova zaženite VM in preskusite znova. 
2. Preverite nastavitve omrežja VM, da ugotovite, ali imate za blokiranje prometa varnostne skupine omrežja (NSGs). Uporabite lahko tudi orodje za preverjanje [pretoka IP omrežja v omrežju](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) , če želite preveriti, ali je NSGs blokiral promet, User-Defined smeri (UDRs) preusmerjanje prometa na mesto na mestu uporabe (» privzeta pot «0.0.0.0/0) ali v omrežno napravo.
Če še vedno prihaja do težav, ko poskušate izvesti zgornje korake, navedite ime VM in vrata TCP, ki jim želite poslati e-pošto za nadaljnjo diagnozo.

**Priporočeni dokumenti**

[Omejitve in priporočila za pošiljanje odhodne e-pošte prek vrat 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)