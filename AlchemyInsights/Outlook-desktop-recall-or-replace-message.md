---
title: Outlook Preklic ali zamenjava e-poštnega sporočila na namizju
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
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918411"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Preklic ali zamenjava Outlook-poštnega sporočila

- Kot skrbnik lahko prekličete sporočila **v imenu uporabnikov, ki uporabljajo PowerShell.** Sporočil iz skrbniškega središča ni mogoče preklicati.
- Prekličete **lahko le sporočila, ki so poslana ljudem v vaši organizaciji.** Če je bilo sporočilo na primer poslano na naslov storitve Gmail, ga ne morete preklicati.
- Sporočila, **poslana iz računalnika s sistemom Windows Outlook 2016 lahko prekličete.** Če uporabnik pošlje sporočilo v Outlook za Mac ali Outlook v spletu, ga ne morete preklicati.

Če želite preklicati ali zamenjati e-poštno sporočilo:

1. V podoknu z mapami na levi strani okna Outlook izberite mapo Poslano.
1. Dvokliknite sporočilo, ki ga želite preklicati, da ga odprete.
1. Izberite **zavihek** Sporočilo in nato **Dejanja** preklica  >  **tega sporočila.**
1. Izberite **Izbriši neprebrane kopije tega sporočila** ali Izbriši **neprebrane kopije** in jih zamenjaj z novim sporočilom , nato pa izberite V **redu**.
1. Če pošiljate nadomestno sporočilo, ga sestavite in izberite **Pošlji**.
1. Uspeh ali neuspeh preklica sporočila je odvisen od prejemnikovih nastavitev v Outlook. Če želite navodila za preverjanje preklica, si oglejte [ta članek.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

Iskanje in brisanje e-poštnih sporočil v organizaciji

- Če niste globalni skrbnik, mora biti vaš račun dodan v vlogo upravitelja e-odkrivanja ali vlogo upravljanja iskanja skladnosti, če želite poiskati sporočila. Če želite izbrisati sporočila, se morate pridružiti skupini vlog za upravljanje organizacije ali vlogi upravljanja iskanja in čiščenja. Dovoljenja za te vloge so dodeljena v središču za varnost in [skladnost s predpisi.](https://go.microsoft.com/fwlink/?linkid=2083731)
- [Ustvarite iskanje vsebine in](https://docs.microsoft.com/microsoft-365/compliance/content-search) poiščite sporočilo, ki ga želite izbrisati.
- [Povezovalnik v Središče za varnost in skladnost s predpisi PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

Če uporabljate večkratno preverjanje pristnosti, glejte Povezovalnik za Microsoft 365 in skladnost s predpisi PowerShell z večkratno [preverjanjem pristnosti.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)