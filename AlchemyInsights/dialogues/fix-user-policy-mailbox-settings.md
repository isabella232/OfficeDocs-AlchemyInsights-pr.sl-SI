---
title: Popravljanje uporabniških pravilnikov/nastavitev nabiralnika
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695901"
---
# <a name="fix-user-policymailbox-settings"></a>Popravljanje uporabniških pravilnikov/nastavitev nabiralnika

Nastavitve neželene pošte v nabiralniku so vplivale na to sporočilo. Če želite pregledati nastavitve, naredite to:

1. Zaženite ukazno lupino za upravljanje Exchangea. Če želite več informacij, glejte [odpiranje lupine za upravljanje Exchangea](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Zaženite ta ukaz (z uporabo e-poštnega naslova uporabnika):  **Get-mailboxjunkmailconfiguration-Identity "User@domain.com"**
3. Preverite, ali je pošiljateljev e-poštni naslov del **TrustedSendersAndDomains** ali **BlockedSendersAndDomains**. Če je e-poštni naslov na enem od seznamov, ga boste morda morali odstraniti. Če želite izvedeti več, glejte [set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
