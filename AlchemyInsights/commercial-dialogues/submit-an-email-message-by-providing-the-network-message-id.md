---
title: Pošiljanje e-poštnega sporočila z zagotavljanjem ID-ja omrežnega sporočila
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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748208"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>Pošiljanje e-poštnega sporočila z zagotavljanjem ID-ja omrežnega sporočila

1. V **novi oddaji** flyout izberite **e-pošta** in **omrežni ID sporočila**.
2. Če želite poiskati ID sporočila za e-poštno sporočilo v Outlooku, upoštevajte ta navodila:
    1. Dvokliknite e-poštno sporočilo, da ga odprete.
    1. Izberite   >  **lastnosti** datoteke.
    1. Odprite beležnico ali prazen Wordov dokument in nato kopirajte in prilepite vsebino, ki je na voljo v polju **Internetne glave** , v odprt dokument za boljšo vidljivost.
    1. Poiščite polje **X-MS-Exchange-Organization-Network-ID sporočila** . Vrednost za **:** je ID, ki ga potrebujete za vašo predložitvi.
3. V razdelku **prejemniki**, če je e-pošta, iztovorjena v mapi» Neželena pošta «za vse prejemnike te e-pošte, izberite **Izberi vse**. Če niste, izberite le uporabnik, ki je sporočil težavo.
4. V **razdelku razlog za pošiljanje**, če ste izbrali **bi morali biti blokirani**, določite, ali naj bo sporočilo blokirano kot **neželena pošta**, **lažno predstavljanje** ali **zlonamerna programska oprema**, nato pa izberite **Pošlji**.

Če želite izvedeti več, glejte [pošiljanje domnevnih neželene pošte, Phish, URL-jev in datotek Microsoftu za skeniranje](https://go.microsoft.com/fwlink/?linkid=2101479).
