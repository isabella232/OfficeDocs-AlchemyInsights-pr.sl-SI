---
title: Outlook Desktop Prekliči ali Zamenjaj e-poštno sporočilo
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664006"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Preklic ali zamenjava Outlookovega e-poštnega sporočila

- Kot skrbnik lahko v **imenu uporabnikov, ki uporabljajo PowerShell**, prekličete sporočila. Ne morete se spomniti sporočil v skrbniškem središču.
- **Sporočila, ki so poslana osebam v organizaciji, lahko odpokličete le**. Če je bilo sporočilo poslano na naslov Gmail, ga na primer ne morete preklicati.
- Sporočila, **poslana iz programa Outlook 2016**, lahko prekličete le v računalniku s sistemom Windows. Če uporabnik pošlje sporočilo z Outlookom za Mac ali Outlookom v spletu, ga ne morete preklicati.

Če želite preklicati ali zamenjati e-poštno sporočilo:

1. V podoknu» mapa «na levi strani Outlookovega okna izberite mapo Poslano.
1. Dvokliknite sporočilo, ki ga želite preklicati, da ga odprete.
1. Izberite zavihek **sporočilo** , nato pa izberite **dejanja**  >  **Prekliči to sporočilo**.
1. Izberite **Izbriši neprebrane kopije tega sporočila** ali **Izbriši neprebrane kopije in jih Zamenjaj z novim sporočilom**, nato pa izberite **v redu**.
1. Če pošiljate nadomestno sporočilo, sestavite sporočilo in nato izberite **Pošlji**.
1. Uspeh ali neuspeh odpoklica sporočil je odvisen od nastavitev prejemnika v Outlooku. Če želite navodila za preverjanje odpoklica, glejte [Ta članek](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Iskanje in brisanje e-poštnih sporočil v organizaciji

- Če niste globalni skrbnik, mora biti vaš račun dodan v vlogo upravitelja E-odkrivanje ali upravljanje iskanja skladnosti, če želite poiskati sporočila. Če želite izbrisati sporočila, se morate vključiti v skupino vlog za upravljanje organizacije ali vlogo za upravljanje iskanja in čiščenja. Dovoljenja za te vloge so dodeljena v [središču za varnost in skladnost s predpisi](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Ustvarite iskanje vsebine](https://docs.microsoft.com/microsoft-365/compliance/content-search) , da poiščete sporočilo, ki ga želite izbrisati.
- [Povežite se s središčem PowerShell za varnost in skladnost s predpisi](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Če uporabljate več dejavnikov preverjanja pristnosti, si oglejte [povezovanje z lupino za varnost in skladnost s programom Microsoft 365 z uporabo več dejavnikov preverjanja pristnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).