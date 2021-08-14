---
title: Samodejno šifriranje določenih e Office 365-poštnih sporočil
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
ms.openlocfilehash: 8ae1c6853f41790efc3b24a9dc696bccf8385967d8c9219a1200e287e6ce32a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53949583"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a>Samodejno šifriranje določenih e Office 365-poštnih sporočil

Sporočila, ki jih uporabniki pošiljajo določenim zunanjim ljudem ali organizacijam, lahko samodejno šifrirate. To naredite tako:

1. V [skrbniškem središču Exchange](https://outlook.office365.com/ecp/)izberite tok **pošte > pravila.** 
2. Kliknite ikono **Novo (+),** nato pa kliknite **Uporabi zaščito šifriranje sporočil v storitvi Office 365 in zaščito pravic v sporočilih.**
3. V **polje** Ime vnesite ime pravila, na primer Šifriraj sporočila, *poslana DrToniRamos@gmail.com*.
4. V **razdelku Uporabi to pravilo, če** izberite Ime > je ta **oseba.** 
5. V **oknu Izbira** članov izberite ime osebe, za katero želite uporabiti šifrirno pravilo, in nato kliknite **dodaj**. 
6. Ko dodate uporabnike, kliknite V **redu.**
7. Ob polju **Naredi to kliknite** Izberi eno **možnost**. 
8. V **spustnem meniju** predloge RMS izberite Šifriraj in nato kliknite V **redu.**  (Če ta možnost ni na voljo, vaš paket ne vključuje samodejnega šifriranja. Lahko pa jo dodate.)
9. Izberite poljuben izbirni izbor (na seznamu izbirnih izborov, ki jih lahko izberete na tej točki, številni izbori pa lahko zaradi preprostosti izberejo privzeto nastavitev).
10. Kliknite **Shrani**.

> [!IMPORTANT]
> To pravilo lahko vedno uredite pozneje.

Če želite več informacij o ustvarjanju pravil za šifriranje, glejte Določanje pravil toka pošte [za šifriranje e-poštnih sporočil v Office 365.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

