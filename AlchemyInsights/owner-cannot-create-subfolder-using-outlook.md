---
title: Lastnik ne more ustvariti podmape z Outlookom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749145"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Lastnik ne more ustvariti podmape z Outlookom

**V programu Outlook je Trenutna težava z lastniki javnih map, ki ustvarjajo podmape. Vprašanje bo kmalu določeno.**

Medtem, raba nedoločni zaimek od sledeč workarounds:

1. Uporabite Outlook za MAC ustvariti podmapo, kot je vprašanje vpliva samo Outlook za namizne okna (vse različice)
2. Ali admin ustvariti podmapo z uporabo EXO Shell ali EAC
3. Spremenite DefaultPublicFolderMailbox/Efetivepublicfoldermailbox na uporabnika v drug nabiralnik kot nabiralnik vsebine za mapo, ki povzroča težavo  
    - *Set-poštni nabiralnik UPORABNIK1 DefaultPublicFolderMailbox PubMBX3*
4. Počakajte eno uro, znova zaženite Outlookovo stranko