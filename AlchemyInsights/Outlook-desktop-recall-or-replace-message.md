---
title: Razgled pult odpoklic ali Zamenjaj e-pošto
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389783"
---
# <a name="recall-or-replace-an-email-message"></a>Preklic ali zamenjava e-pošto

- Kot admin, lahko **odpoklic sporočila v imenu uporabnik using PowerShell**. Sporočila iz centra za admin ne more spomniti.
- Lahko **samo Preklic sporočila, ki so poslana ljudem v organizaciji**. Če je bilo sporočilo poslano na Gmail naslov, na primer, lahko ne spomnim to.
- Lahko **samo Preklic sporočila, poslana iz Outlook 2016 na PC**. Če uporabnik pošlje sporočilo z uporabo Outlook za Mac ali Outlook v spletu, lahko spomnim.

Preklicu ali zamenjavi e-pošto:

1. V podoknu z mapami na levi strani Outlookovega okna, izberite mapo Poslano.
1. Dvokliknite sporočilo, da želite preklicati razkleniti to.
1. Izberite **sporočilo** , in nato izberite **dejanja** > **Opozoriti na to sporočilo**.
1. Izberite **izbrisati neprebrane kopije tega sporočila** ali **izbrisati neprebrane kopije in zamenjati z novim sporočilom**in izberite **OK**.
1. Če pošiljate sporočilo zamenjavo, sestaviti sporočilo in izberite **Pošlji**.
1. Uspeh ali neuspeh Preklic sporočila je odvisna od prejemnika nastavitve v Outlooku. Koraki za preverjanje na odpoklic, glejte [Ta članek](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Iskanje in brisanje e-poštnih sporočil v vaši organizaciji

- Če niste svetovnih admin, mora vaš račun dodan eDiscovery vlogo upravitelja ali skladnost iskanje upravljalne vloge za iskanje sporočil. Èe ¾elite zbrisati sporoèila, boste morali pridružiti skupine vlog »Upravljanje organizacije «ali iskanje in Počisti upravljalne vloge. Dovoljenja za te vloge so dodeljeni v [center za varnost in skladnost](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Ustvari vsebino iskanje](https://docs.microsoft.com/office365/securitycompliance/content-search) najti sporočilo za brisanje.
- [Povezati varnost in skladnost Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Če uporabljate preverjanje pristnosti multifaktorske, glejte [povezovanje Office 365 varnost in skladnost Center PowerShell uporablja preverjanje pristnosti multifaktorske](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).