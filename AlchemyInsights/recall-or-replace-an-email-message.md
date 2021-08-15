---
title: Preklic ali zamenjava e-poštnega sporočila
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024402"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Preklic ali zamenjava e-poštnega sporočila v Microsoft 365

- Prekličete **lahko le sporočila, ki so poslana ljudem v vaši organizaciji.** Če je bilo na primer sporočilo poslano na naslov gmail, ga ne morete preklicati.
- Sporočila, **poslana iz računalnika Outlook lahko prekličete.** Če uporabnik pošlje sporočilo v Outlook za Mac ali Outlook v spletu, ga ne morete preklicati.
- Kot skrbnik najemnika lahko prekličete sporočila v imenu uporabnikov tako, da uporabite **PowerShell** (Če želite več informacij, glejte: Iskanje in brisanje [e-poštnih sporočil).](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- Sporočil iz skrbniškega središča ni mogoče preklicati. Če želite več informacij, se pomaknite navzdol do možnosti »Poiščite in izbrišite e-poštna sporočila v organizaciji«.

**Preklic ali zamenjava poslanega e-poštnega sporočila**

1. V podoknu z mapami na levi Outlook izberite mapo Poslano.
2. Odprite sporočilo, ki ga želite preklicati. Če želite sporočilo odpreti, ga morate dvoklikniti. Če sporočilo izberete tako, da je prikazano v podoknu za branje, ga ne boste več lahko preklicali.
3. Na zavihku Sporočilo izberite Dejanja  >  **preklica tega sporočila.**
4. Izberite **Izbriši neprebrane kopije tega sporočila** ali Izbriši **neprebrane kopije** in jih zamenjaj z novim sporočilom , nato pa izberite V **redu**.
5. Če pošiljate nadomestno sporočilo, ga sestavite in izberite **Pošlji**.
6. Uspeh ali neuspeh preklica sporočila je odvisen od prejemnikovih nastavitev v Outlook.

Če želite več informacij, vključno s tem, kako preverite preklic, glejte [Preklic ali zamenjava poslanega e-poštnega sporočila.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Če želite poiskati in izbrisati e-poštna sporočila*** v svoji organizaciji, je najlažje, če ste globalni skrbnik. Če niste globalni skrbnik, mora biti vaš račun dodan v skupino vlog upravitelja e-odkrivanja ali vlogo upravljanja iskanja skladnosti. Če želite izbrisati sporočila, se morate pridružiti skupini vlog za upravljanje organizacije ali vlogi upravljanja iskanja in čiščenja. Dovoljenja za te vloge so dodeljena v središču za varnost in [& za skladnost s predpisi.](https://protection.office.com/)

1. [Ustvarite iskanje vsebine in](https://docs.microsoft.com/microsoft-365/compliance/content-search) poiščite sporočilo, ki ga želite izbrisati.
2. [Povezovalnik središču za & za skladnost s predpisi PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Če uporabljate MFA (Multi-Factor Authentication), si oglejte Povezovalnik, Microsoft 365 Središče za skladnost s predpisi & s storitvijo [Multi-Factor Authentication.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
