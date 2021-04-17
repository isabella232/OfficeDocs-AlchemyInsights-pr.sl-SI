---
title: Lastnik ne more ustvariti podmape z Outlookom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836151"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Lastnik ne more ustvariti podmape z Outlookom

**Trenutno obstaja težava z ustvarjanjem podmap v Outlooku z lastniki javnih map. Ta težava bo kmalu odpravljena.**

Medtem pa uporabite eno od teh rešitev:

1. Uporabite Outlook za MAC, da ustvarite podmapo, saj težava vpliva le na Outlook za namizno različico okna (vse različice)
2. Naj skrbnik ustvari podmapo z lupino EXO ali EAC
3. Spreminjanje mape DefaultPublicFolderMailbox/EffectivePublicFolderMailbox za uporabnika v drug nabiralnik in ne v nabiralnik vsebine za mapo, ki povzroča težavo  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Počakajte eno uro, znova zaženite Outlookovega odjemalca