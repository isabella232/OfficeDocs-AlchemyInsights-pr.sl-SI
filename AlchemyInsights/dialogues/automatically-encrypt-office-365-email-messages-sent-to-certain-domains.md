---
title: Samodejno šifriranje e-poštnih sporočil v storitvi Office 365, poslanih določenim domenam
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526698"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Samodejno šifriranje e-poštnih sporočil v storitvi Office 365, poslanih določenim domenam

1. V [skrbniškem središču za Exchange](https://outlook.office365.com/ecp/)izberite **pravila toka pošte >**. 
2. Kliknite ikono **novo (+)** , nato pa kliknite **uporabi šifriranje sporočil sistema Office 365 in zaščito pravic za sporočila**.
3. V polje **ime** vnesite ime za pravilo, na primer *šifriranje sporočil, poslanih v contoso.com*.
4. **Če želite uporabiti to pravilo, če** izberite **domeno prejemnika >**. 
5. Vnesite ime domene, na primer **contoso.com**.
6. Kliknite ikono **Dodaj (+)** in nato kliknite **v redu**.
7. Poleg polja **naredi to** kliknite **Izberi eno**. 
8. V spustnem meniju **predloga RMS** izberite **Šifriraj** in nato kliknite **v redu**. (Če ne vidite te možnosti, to pomeni, da vaš paket ne vključuje samodejnega šifriranja. Vendar ga lahko dodate!)
9. Izberite poljuben izbirni izbor (na seznamu izbirnih izbir, ki jih lahko naredite na tej strani, od katerih jih je mogoče preprostiti s privzeto nastavitev za enostavnost).
10. Kliknite **Shrani**.

> [!IMPORTANT]
> Pozneje se lahko vrnete in uredite to pravilo.

Če želite več informacij o ustvarjanju pravil za šifriranje, glejte [določanje pravil pretoka pošte za šifriranje e-poštnih sporočil v storitvi Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)