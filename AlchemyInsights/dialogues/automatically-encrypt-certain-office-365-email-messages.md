---
title: Samodejno šifriranje določenih e-poštnih sporočil sistema Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526742"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Samodejno šifriranje določenih e-poštnih sporočil sistema Office 365

Samodejno lahko šifrirate sporočila, ki jih uporabniki pošiljajo določenim zunanjim osebam ali organizacijam. To naredite tako, da izvedete te korake:

1. V [skrbniškem središču za Exchange](https://outlook.office365.com/ecp/)izberite **pravila toka pošte >**. 
2. Kliknite ikono **novo (+)** , nato pa kliknite **uporabi šifriranje sporočil sistema Office 365 in zaščito pravic za sporočila**.
3. V polje **ime** vnesite ime za pravilo, na primer *šifriranje sporočil, poslanih v DrToniRamos@gmail.com*.
4. **Če želite uporabiti to pravilo, če** izberite **prejemnik > je ta oseba**. 
5. V oknu **Izberite člane** izberite ime osebe, za katero želite uporabiti pravilo šifriranja, in nato kliknite **Dodaj**. 
6. Ko končate Dodajanje uporabnikov, kliknite **v redu**.
7. Poleg polja **naredi to** kliknite **Izberi eno**. 
8. V spustnem meniju **predloga RMS** izberite **Šifriraj** in nato kliknite **v redu**. (Če ne vidite te možnosti, to pomeni, da vaš paket ne vključuje samodejnega šifriranja. Vendar ga lahko dodate!)
9. Izberite poljuben izbirni izbor (na seznamu izbirnih izbir, ki jih lahko naredite na tej strani, od katerih jih je mogoče preprostiti s privzeto nastavitev za enostavnost).
10. Kliknite **Shrani**.

> [!IMPORTANT]
> Pozneje se lahko vrnete in uredite to pravilo.

Če želite več informacij o ustvarjanju pravil za šifriranje, glejte [določanje pravil pretoka pošte za šifriranje e-poštnih sporočil v storitvi Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

