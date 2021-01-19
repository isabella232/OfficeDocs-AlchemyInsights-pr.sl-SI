---
title: Krmilnik domene
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901314"
---
# <a name="domain-controller"></a>Krmilnik domene

**Ne morete omogočiti ZVOČNIh naprav – DS ali uvedbe ni mogoče**

Če želite odpraviti težavo z domensko storitvijo Azure AD (ZVOČNa-DS), ki ni omogočena ali ni bila uvedena, izvedite te korake:

1. Če uporabljate že obstoječo navidezno omrežje, potrdite NSG za pravila, ki blokirajo vrata, potrebna za sinhronizacijo v storitvi ZVOČNa-DS v portalu https://aka.ms/aadds-networking .
2. Preverite, ali je odgovor na sporočilo o napaki v tem vodniku za odpravljanje težav, ki je na voljo  https://aka.ms/aadds-troubleshoot-enable .
3. Poskusite uporabiti domenske storitve Azure AD v novem navideznem omrežju.
4. Navodila za uvod v priročnik za uvajanje ZVOČNIh naprav – DS, ki je na voljo na spletnem mestu [Vadnica za ustvarjanje domenskih storitev storitve AZURE ad](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Če imate težave z uvajanjem domen v storitvi Azure AD Services, glejte [Odpravljanje težav z domenami storitve AZURE ad](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , da odpravite pogoste napake, s katerimi lahko znova začnete delati. 

**Ne morete onemogočiti ZVOČNIh-DS**

ZVOČNa-DS ne more biti začasno ustavljena. Če želite prenehati uporabljati upravljano domeno, jo morate izbrisati.

Če naletite na težave, razrešite pogosta sporočila o napakah in povezane korake za odpravljanje težav, ki vam bodo v pomoč pri ponovnem zagonu, glejte [Odpravljanje težav z domenami storitve Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
