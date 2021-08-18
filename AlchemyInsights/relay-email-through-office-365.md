---
title: Posredovanje e-pošte prek okolja Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 8f8b0780ebec2911b6698deee25e0fabe83bd9afef5fb3a6ef4c51cccd67fc7c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898564"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Nastavite večfunkcijsko napravo ali aplikacijo za pošiljanje e-pošte

Več informacij o možnostih in navodila najdete v članku [Nastavitev večfunkcijske naprave ali aplikacije za pošiljanje e-pošte z okoljem Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Če imate napravo ali aplikacijo, ki je nedavno prenehala delovati, so najpogostejše težave:

- **Napake, povezane s preverjanjem pristnosti pri uporabi pošiljanja SMTP Auth odjemalca** Nedavno smo naredili nekaj sprememb, povezanih z načinom dela preverjanja pristnosti SMTP. Če želite več informacij o odpravljanju težav, glejte razdelek o neuspešnem preverjanju pristnosti v razdelku Odpravljanje težav s tiskalniki, optičnimi bralniki in programi LOB, ki pošiljajo e-pošto s programom [Microsoft 365 ali Office 365.](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)
- **Sprejemamo le različico TLS 1.2, medtem** ko pripravljamo varno povezavo za Office 365 Če uporabljate varno povezavo (TLS), se prepričajte, da aplikacija podpira TLS 1.2. Če želite več informacij, [glejte Priprava na TLS 1.2](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)v Office 365 in Office 365 GCC.
 
Če želite druge težave in rešitve, glejte Odpravljanje težav s [tiskalniki,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)optičnimi bralniki in aplikacijami LOB, ki pošiljajo e-pošto Microsoft 365 ali Office 365.

Če si želite ogledati prizadete naprave, pojdite na[ Poročilo o odjemalcih s preverjanjem pristnosti SMTP Auth](https://protection.office.com/mailflow/dashboard).

**Opomba:** Exchange Online primeri množične pošte niso na voljo. Če želite poslati množično komercialno e-pošto (na primer glasila strank), uporabite tretje ponudnike, ki so posebni za te storitve.
