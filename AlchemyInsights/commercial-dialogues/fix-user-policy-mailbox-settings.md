---
title: Odpravljanje težav s pravilnikom uporabnika/nastavitvami nabiralnika
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034734"
---
# <a name="fix-user-policymailbox-settings"></a>Odpravljanje težav s pravilnikom uporabnika/nastavitvami nabiralnika

Nastavitve neželene pošte v nabiralniku so vplivale na to sporočilo. Če želite pregledati nastavitve, naredite to:

1. Zaženite Exchange za upravljanje. Če želite več informacij, glejte [Odpiranje ukazne lupine Exchange za upravljanje sistema .](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Zaženite ta ukaz (z e-poštnim naslovom uporabnika):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Preverite, ali je e-poštni naslov pošiljatelja del **storitev TrustedSendersAndDomains** ali **BlockedSendersAndDomains.** Če je e-poštni naslov na enem od seznamov, ga boste morda morali odstraniti. Če želite izvedeti več, [glejte Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
