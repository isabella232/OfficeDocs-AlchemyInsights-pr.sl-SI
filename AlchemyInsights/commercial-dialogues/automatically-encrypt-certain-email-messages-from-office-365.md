---
title: Samodejno šifriranje določenih e-poštnih sporočil v storitvi Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749456"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Samodejno šifriranje določenih e-poštnih sporočil v storitvi Office 365

1. V [skrbniškem središču za Exchange](https://outlook.office365.com/ecp/)izberite **pravila toka pošte >**. 
2. Kliknite ikono **novo (+)** , nato pa kliknite **uporabi šifriranje sporočil sistema Office 365 in zaščito pravic za sporočila**.
3. V polje **ime** vnesite ime za pravilo, na primer *Šifriraj vsa sporočila*.
4. **Če želite uporabiti to pravilo**, izberite **[uporabi za vsa sporočila]**. 
5. Poleg polja **naredi to** kliknite **Izberi eno**. 
6. V spustnem meniju **predloga RMS** izberite **Šifriraj** in nato kliknite **v redu**. (Če ne vidite te možnosti, to pomeni, da vaš paket ne vključuje samodejnega šifriranja. Vendar ga lahko dodate!)
7. Potrdite potrditveno polje **Nadziraj to pravilo z ravnjo resnosti** in nato izberite želeno raven. Če ima vaše podjetje pogodbene obveznosti, da pošljejo vsa šifrirana e-poštna sporočila, vam priporočam, da nastavite raven na **visoko**.
8. V razdelku **Izberite model za to pravilo** kliknite **Uveljavi**. 
9. Izberite poljuben izbirni izbor (na seznamu izbirnih izbir, ki jih lahko naredite na tej strani, od katerih jih je mogoče preprostiti s privzeto nastavitev za enostavnost).
10. Kliknite **Shrani**.

> [!IMPORTANT]
> Pozneje se lahko vrnete in uredite to pravilo.

Če želite več informacij o ustvarjanju pravil za šifriranje, glejte [določanje pravil pretoka pošte za šifriranje e-poštnih sporočil v storitvi Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

