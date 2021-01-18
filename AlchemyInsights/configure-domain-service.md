---
title: Konfiguracija storitve Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885687"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Ne morete omogočiti ZVOČNIh naprav – DS ali uvedbe ni mogoče

Če želite odpraviti težavo z domensko storitvijo Azure AD (ZVOČNa-DS), ki ni omogočena ali ni bila uvedena, izvedite te korake:

1. Če uporabljate že obstoječo navidezno omrežje, potrdite NSG za pravila, ki blokirajo vrata, potrebna za sinhronizacijo v storitvi ZVOČNa-DS v portalu https://aka.ms/aadds-networking .
2. Preverite, ali je odgovor na sporočilo o napaki v tem vodniku za odpravljanje težav, ki je na voljo  https://aka.ms/aadds-troubleshoot-enable .
3. Poskusite uporabiti domenske storitve Azure AD v novem navideznem omrežju.
4. Navodila za začetek vodnika za uvajanje ZVOČNIh [storitev](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. Če imate težave z uvajanjem domen v storitvi Azure AD Services, glejte [Odpravljanje težav z domenami storitve AZURE ad](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , da odpravite pogoste napake, s katerimi lahko znova začnete delati. 

**Ne morete onemogočiti ZVOČNIh-DS**

ZVOČNa-DS ne more biti začasno ustavljena. Če želite prenehati uporabljati upravljano domeno, jo morate izbrisati.
Če želite izbrisati upravljano domeno, si oglejte [brisanje storitve v storitvi zvočna domena](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



