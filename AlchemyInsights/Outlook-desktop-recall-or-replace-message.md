---
title: Outlook Desktop se spomni ali zamenja e-poštno sporočilo
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687526"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Odpoklic ali zamenjava Outlookovega e-poštnega sporočila

- Kot admin, lahko **odpoklic sporočil v imenu uporabnikov, ki uporabljajo PowerShell**. Ne morete se spomniti sporočil iz skrbniškega centra.
- Prikličete lahko **samo sporočila, poslana osebam v vaši organizaciji**. Če je bilo sporočilo poslano v Gmailov naslov, ga na primer ne morete spomniti.
- **V računalniku lahko odpokličejo samo sporočila, poslana iz outlooka 2016**. Če uporabnik pošlje sporočilo z Outlookom za Mac ali Outlook v spletu, ga ne morete spomniti.

Preklic ali zamenjava e-poštnega sporočila:

1. V podoknu map na levi strani Outlookovega okna izberite mapo Poslani predmeti.
1. Dvokliknite sporočilo, ki ga želite opomniti, da ga odprete.
1. Izberite zavihek **sporočilo** in nato izberite **dejanja** > , ki se**odpokličejo v to sporočilo**.
1. Izberite **Izbriši neprebrane kopije tega sporočila** ali **izbrišite neprebrane kopije in zamenjajte novo sporočilo**, nato pa izberite **v redu**.
1. Če pošiljate nadomestno sporočilo, sestavite sporočilo in nato izberite **Pošlji**.
1. Uspeh ali neuspeh odpoklica sporočila je odvisen od prejemnikov nastavitev v programu Outlook. Če želite preveriti odpoklic, si oglejte [Ta članek](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Iskanje in brisanje e-poštnih sporočil v organizaciji

- Če niste globalni skrbnik, morate račun dodati vlogi upravitelja e-odkrivanja ali vlogi za upravljanje iskanja po skladnosti za iskanje sporočil. Če želite izbrisati sporočila, se morate pridružiti skupini vlog za upravljanje organizacije ali funkciji za upravljanje iskanja in čiščenja. Dovoljenja za te vloge so dodeljena v [središču za varnost in skladnost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Ustvarite iskanje po vsebini](https://docs.microsoft.com/office365/securitycompliance/content-search) in poiščite sporočilo, ki ga želite izbrisati.
- [Vzpostavite povezavo z lupino za varnostno in skladnost center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Če uporabljate večfaktorsko preverjanje pristnosti, glejte [Vzpostavljanje povezave z Microsoft 365 varnostjo in lupino središča za skladnost z uporabo večfaktorskega preverjanja pristnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).