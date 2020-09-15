---
title: Manjkajoča e-poštna sporočila v karanteni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673730"
---
# <a name="missing-emails-in-quarantine"></a>Manjkajoča e-poštna sporočila v karanteni

Skrbniki [si lahko ogledajo, izdajajo ali izbrišejo ta sporočila.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Če želite odpreti središče za skladnost varnostnega &, pojdite na [https://protection.office.com](https://protection.office.com/) . Če želite odpreti stran karantene neposredno, pojdite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Iščete lahko po teh vrednostih:  

- **ID sporočila**: globalni enolični identifikator sporočila. Če izberete sporočilo na seznamu, se prikaže vrednost  **ID sporočila**  v podoknu  **podrobnosti**  flyout, ki se prikaže. Skrbniki lahko s [sledenjem sporočil](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) poiščejo sporočila in njihove ustrezne vrednosti ID-ja sporočila.
- **Pošiljatelj e-poštni naslov**: e-poštni naslov enega pošiljatelja.
- **E-poštni naslov prejemnika**: e-poštni naslov posameznega prejemnika.
- **Zadeva**: uporabite celotno zadevo sporočila. Iskanje ne razlikuje med velikimi in malimi črkami.

Ko vnesete pogoje iskanja, kliknite Osveži gumb Osveži, ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** da filtrirate rezultate.  

Ukazi» cmdlet «, ki jih uporabljate za ogled in upravljanje sporočil in datotek v karanteni, so:
- [Izbriši-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Predogled – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Upoštevajte, da je ta ukaz» cmdlet «le za sporočila in ne zlonamerne programske opreme v storitvi ATP za SharePoint online, OneDrive za podjetja ali teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)