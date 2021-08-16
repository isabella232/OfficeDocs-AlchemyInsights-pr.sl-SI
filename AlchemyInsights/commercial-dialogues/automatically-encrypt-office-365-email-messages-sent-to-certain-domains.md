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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082202"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Samodejno šifriranje Office 365 sporočil, poslanih v določene domene

1. V [skrbniškem središču Exchange](https://outlook.office365.com/ecp/)izberite tok **pošte > pravila.** 
2. Kliknite ikono **Novo (+),** nato pa kliknite **Uporabi zaščito šifriranje sporočil v storitvi Office 365 in zaščito pravic v sporočilih.**
3. V **polje** Ime vnesite ime pravila, na primer Šifriraj sporočila, *poslana contoso.com.*
4. V **razdelku Uporabi to pravilo, če** izberite **Prejemnikova domena > je**. 
5. Vnesite ime domene, na primer **ime contoso.com.**
6. Kliknite **ikono Dodaj (+)** in nato V **redu.**
7. Ob polju **Naredi to kliknite** Izberi eno **možnost**. 
8. V **spustnem meniju** predloge RMS izberite Šifriraj in nato kliknite V **redu.**  (Če ta možnost ni na voljo, vaš paket ne vključuje samodejnega šifriranja. Lahko pa jo dodate.)
9. Izberite poljuben izbirni izbor (na seznamu izbirnih izborov, ki jih lahko izberete na tej točki, številni izbori pa lahko zaradi preprostosti izberejo privzeto nastavitev).
10. Kliknite **Shrani**.

> [!IMPORTANT]
> To pravilo lahko vedno uredite pozneje.

Če želite več informacij o ustvarjanju pravil za šifriranje, glejte Določanje pravil toka pošte [za šifriranje e-poštnih sporočil v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)