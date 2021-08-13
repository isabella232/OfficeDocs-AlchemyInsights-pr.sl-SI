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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974973"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premikanje e-pošte v nabiralnik arhiva

Če želite, da zaženemo avtomatizirana preverjanja za spodaj omenjene nastavitve, izberite gumb »Nazaj« < – na vrhu te strani in nato vnesite e-poštni naslov uporabnika, ki ima težave s premikanjem e-pošte v nabiralnik arhiva.

1. Preverite, ali **je nabiralnik** arhiva omogočen. Če ni, sledite korakom v tem [članku, da](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) omogočite nabiralnik arhiva.

2. Če želite sporočila samodejno arhivirati v nabiralnik  arhiva, morate nastaviti oznako za hranjenje z dejanjem Premakni v arhiv, da bo samodejno uporabljena za celotno oznako **nabiralnika (privzeto).** Uporabite navodila tukaj, da ustvarite oznako: [Arhiviraj privzeto oznako](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Nato pravilniku o **hranjenju** dodajte oznako Arhiv. V skrbniškem središču Exchange izberite **Pravilniki** o hranjenju, da > pravilniku dodate oznako Premakni v arhiv, > **Shrani.** 

4. Zdaj [dodelite pravilnik o](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) hranjenju določenemu nabiralniku uporabnika. Isti pravilnik bo uporabljen tako za nabiralnik primarnega **kot** tudi za **nabiralnik arhiva.**

Pomočnika za upravljane mape bo morda moral zagnati in uporabiti nove nastavitve za nabiralnik uporabnika. Zaženite ta ukaz, ko [imate vzpostavljeno povezavo z EXO PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da zaženete pomočnika za upravljane mape za določen nabiralnik:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Če želite več informacij o nastavitvi pravilnika arhiva, glejte [Nastavitev pravilnika o arhiviranja in brisanju za nabiralnike.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  