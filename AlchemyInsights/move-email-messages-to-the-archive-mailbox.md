---
title: Premikanje e-poštnih sporočil v nabiralnik arhiviranja
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522787"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premikanje e-pošte v arhivski nabiralnik

Če želite, da zaženemo samodejne preglede za spodaj navedene nastavitve, izberite gumb za nazaj < - na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave pri premikanju e-pošte v svoj arhivski nabiralnik.

1. Preverite, ali **je bil nabiralnik** arhiva omogočen. Če ne, uporabite korake v [tem članku,](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da omogočite arhivski nabiralnik.

2. Če želite samodejno arhivirati sporočila v arhivski nabiralnik, mora biti oznaka hranjenja **z dejanjem »Premakni** v arhiv« nastavljena na **samodejno uporabljeno za celotno oznako nabiralnika (privzeto).** Če želite ustvariti oznako: Arhiv privzete oznake [uporabite tukaj](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Nato v pravilnik o **hranjenju** dodajte oznako Arhiv. V Skrbniškem središču za Exchange izberite **Pravilniki** o hranjenju > dodajte **oznako Premakni** v arhiv v pravilnik > **Shrani**.

4. Zdaj [dodelite pravilnik o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nabiralniku določenega uporabnika. Enak pravilnik bo uporabljen za nabiralnik **»Primarni« in** **»Arhiv«.**

Morda bo treba pomočnika za upravljane mape (MFA) prisiliti, da zažene in uporabi nove nastavitve v uporabnikovem nabiralniku. Ko ste povezani z lupino [EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) zaženite ta ukaz, da zaženete pomočnika za upravljane mape za določen nabiralnik:
  
Start-ManagedFolderAssistant -Identiteta<name of the mailbox>

Če želite več informacij o nastavitvi pravilnika arhiva, [glejte Nastavitev pravilnika arhiva in brisanja nabiralnikov](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  