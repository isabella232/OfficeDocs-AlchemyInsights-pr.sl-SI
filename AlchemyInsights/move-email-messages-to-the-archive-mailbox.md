---
title: Premikanje e-poštnih sporočil v nabiralnik arhiva
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799796"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premikanje e-pošte v arhivski nabiralnik

Če želite, da zaženemo avtomatizirane kontrole za spodaj navedene nastavitve, izberite gumb» Vrni «< na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave s premikanjem e-pošte v svoj arhivski nabiralnik.

1. Preverite, ali je bil **nabiralnik v arhivu** omogočen. V nasprotnem primeru uporabite korake v [tem članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) , da omogočite arhivski nabiralnik.

2. Če želite samodejno arhivirati sporočila v arhivski nabiralnik, mora biti oznaka za hranjenje s dejanjem» **Premakni v Arhiv** «nastavljena tako, da se **samodejno uporabi za celoten nabiralnik (privzeta) oznaka**. Uporabite korake tukaj, če želite ustvariti oznako: [privzeto oznako za arhiviranje](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Nato dodajte oznako **arhiva** v pravilnik o hranjenju. V skrbniškem središču za Exchange izberite **Pravilniki o hranjenju** > dodajte **oznako» Premakni v Arhiv** «v pravilnik > **Shrani**.

4. Zdaj [dodelite pravilnik o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) v nabiralnik določenega uporabnika. Ista politika bo uporabljena tako v **primarnem** kot v **arhivskem** nabiralniku.

Morda bo treba pognati pomočnika za upravljane mape (MFA), da bo zagnal in uporabil nove nastavitve v nabiralniku uporabnika. Zaženite ta ukaz, medtem ko [imate vzpostavljeno povezavo s storitvijo ekso PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) , da zaženete pomočnika za upravljane mape za določen nabiralnik:
  
Začetna ManagedFolderAssistant – identiteta <name of the mailbox>

Če želite več informacij o nastavljanju pravilnika za arhiviranje, glejte [nastavitev pravilnika za arhiviranje in brisanje nabiralnikov](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  