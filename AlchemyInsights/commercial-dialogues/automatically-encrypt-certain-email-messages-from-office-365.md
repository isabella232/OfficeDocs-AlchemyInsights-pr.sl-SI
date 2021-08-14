---
title: Samodejno šifriranje določenih e-poštnih sporočil iz storitve Office 365
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
ms.openlocfilehash: 74f9733196004fd7a78eeb290c948a9f35ac2a31b3c5b00bf82e44081aac8637
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988851"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a>Samodejno šifriranje določenih e-poštnih sporočil iz storitve Office 365

1. V [skrbniškem središču Exchange](https://outlook.office365.com/ecp/)izberite tok **pošte > pravila.** 
2. Kliknite ikono **Novo (+),** nato pa kliknite **Uporabi zaščito šifriranje sporočil v storitvi Office 365 in zaščito pravic v sporočilih.**
3. V **polje** Ime vnesite ime pravila, na primer *Šifriraj vsa sporočila.*
4. V **razdelku Uporabi to pravilo, če** izberite **[Uporabi za vsa sporočila]**. 
5. Ob polju **Naredi to kliknite** Izberi eno **možnost**. 
6. V **spustnem meniju** predloge RMS izberite Šifriraj in nato kliknite V **redu.**  (Če ta možnost ni na voljo, vaš paket ne vključuje samodejnega šifriranja. Lahko pa jo dodate.)
7. Potrdite **polje Nadziraj to pravilo z resnostjo** in izberite želeno raven. Če ima vaše podjetje pogodbene obveznosti glede pošiljanja vseh šifriranih e-poštnih sporočil, priporočamo, da raven nastavite na **Visoko.**
8. V **razdelku Izberite model za to pravilo** kliknite **Vsili**. 
9. Izberite poljuben izbirni izbor (na seznamu izbirnih izborov, ki jih lahko izberete na tej točki, številni izbori pa lahko zaradi preprostosti izberejo privzeto nastavitev).
10. Kliknite **Shrani**.

> [!IMPORTANT]
> To pravilo lahko vedno uredite pozneje.

Če želite več informacij o ustvarjanju pravil za šifriranje, glejte Določanje pravil toka pošte [za šifriranje e-poštnih sporočil v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)

