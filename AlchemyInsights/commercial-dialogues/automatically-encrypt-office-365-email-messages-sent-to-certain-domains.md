---
title: Samodejno šifriranje Office 365 sporočil, poslanih v določene domene
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
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318864"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Samodejno šifriranje Office 365 sporočil, poslanih v določene domene

1. V [skrbniškem središču Exchange](https://outlook.office365.com/ecp/)izberite tok **pošte in > pošte.** 
2. Kliknite ikono **Novo (+),** nato pa kliknite **Uporabi zaščito šifriranje sporočil v storitvi Office 365 in pravice v sporočilih.**
3. V **polje** Ime vnesite ime pravila, na primer Šifriraj sporočila, *poslana contoso.com.*
4. In **Apply this rule if**, choose The recipient > domain **is**. 
5. Vnesite ime domene, na primer **ime contoso.com.**
6. Kliknite **ikono Dodaj (+)** in nato V **redu.**
7. Ob polju **Naredi to kliknite** Izberi eno **možnost**. 
8. V **spustnem meniju** predloge RMS izberite Šifriraj in nato kliknite V **redu.**  (Če ta možnost ni na voljo, vaš paket ne vključuje samodejnega šifriranja. Lahko pa jo dodate.)
9. Izberite poljuben izbirni izbor (na seznamu izbirnih izborov, ki jih lahko izberete na tej točki, številni izbori pa lahko zaradi preprostosti izberejo privzeto nastavitev).
10. Kliknite **Shrani**.

**Pomembno:** To pravilo lahko vedno uredite pozneje.

Če želite več informacij o ustvarjanju pravil za šifriranje, glejte Določanje pravil toka pošte [za šifriranje e-poštnih sporočil v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)