---
title: Lastnik ne more ustvariti podmape s Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063140"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Lastnik ne more ustvariti podmape s Outlook

**V teku je težava z ustvarjanjem podmap z lastniki javnih map z uporabo Outlook. Ta težava bo kmalu odpravljena.**

Medtem pa uporabite eno od teh rešitev:

1. Uporabite Outlook za MAC, da ustvarite podmapo, saj težava vpliva le na Outlook za namizna okna (vse različice)
2. Naj skrbnik ustvari podmapo z lupino EXO ali EAC
3. Spreminjanje mape DefaultPublicFolderMailbox/EffectivePublicFolderMailbox za uporabnika v drug nabiralnik in ne v nabiralnik vsebine za mapo, ki povzroča težavo  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Počakajte eno uro, znova zaženite Outlookovega odjemalca