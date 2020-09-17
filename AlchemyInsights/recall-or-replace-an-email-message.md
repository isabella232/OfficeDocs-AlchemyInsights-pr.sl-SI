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
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799220"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Preklic ali zamenjava e-poštnega sporočila v programu Microsoft 365

- **Sporočila, ki so poslana osebam v organizaciji, lahko odpokličete le**. Če je bilo sporočilo poslano na naslov Gmail, ga na primer ne morete preklicati.
- Prekličete lahko **le sporočila, poslana iz programa Outlook 2016 za računalnik s**sistemom Windows. Če uporabnik pošlje sporočilo z Outlookom za Mac ali Outlookom v spletu, ga ne morete preklicati.
- Če ste skrbnik, lahko prekličete **sporočila v imenu uporabnikov z uporabo lupine PowerShell**. Ne morete se spomniti sporočil v skrbniškem središču. Če želite več informacij, se pomaknite navzdol do možnosti» iskanje in brisanje e-poštnih sporočil v organizaciji «.

**Preklic ali zamenjava poslanega e-poštnega sporočila**

1. V podoknu» mapa «na levi strani Outlookovega okna izberite mapo Poslano.
2. Odprite sporočilo, ki ga želite preklicati. Če želite odpreti sporočilo, morate dvoklikniti. Če izberete sporočilo, da se prikaže v podoknu za branje, ne boste mogli preklicati sporočila.
3. Na zavihku sporočilo izberite **dejanja**  >  **Prekliči to sporočilo**.
4. Izberite **Izbriši neprebrane kopije tega sporočila** ali **Izbriši neprebrane kopije in jih Zamenjaj z novim sporočilom**, nato pa izberite **v redu**.
5. Če pošiljate nadomestno sporočilo, sestavite sporočilo in izberite **Pošlji**.
6. Uspeh ali neuspeh odpoklica sporočila je odvisen od nastavitev prejemnikov v Outlooku.

Če želite več informacij, vključno s tem, kako preverite preklic, glejte [preklic ali zamenjava e-poštnega sporočila, ki ste ga poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Iskanje in brisanje e-poštnih sporočil v organizaciji*** Če želite poiskati in izbrisati e-poštna sporočila v vaši organizaciji, je najlažje, če ste globalni skrbnik. Če niste globalni skrbnik, mora biti vaš račun dodan v skupino vlog E-odkrivanje Manager ali pa na vlogo za upravljanje iskanja skladnosti. Če želite izbrisati sporočila, se morate vključiti v skupino vlog za upravljanje organizacije ali vlogo za upravljanje iskanja in čiščenja. Dovoljenja za te vloge so dodeljena v [središču za skladnost varnostnega &](https://protection.office.com/).

1. [Ustvarite iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/content-search) , da poiščete sporočilo, ki ga želite izbrisati.
2. [Vzpostavi povezavo z varnostnim središčem v središču za skladnost z varnostjo &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Če uporabljate funkcijo MFA, si oglejte [povezovanje z & varnostnim središčem za skladnost s storitvijo Microsoft 365, ki uporablja več kot preverjanje pristnosti z več dejavniki](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
