---
title: Manjkajoča e-poštna sporočila v karanteni
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831750"
---
# <a name="missing-emails-in-quarantine"></a>Manjkajoča e-poštna sporočila v karanteni«

Skrbniki si lahko [ogledajo ta sporočila, jih izdajajo ali izbrišejo.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Če želite odpreti Središče & za skladnost s predpisi, odprite [https://protection.office.com](https://protection.office.com/) . Če želite stran Karantena odpreti neposredno, odprite [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Iščete lahko po teh vrednostih:  

- **ID sporočila:** globalni enolični identifikator sporočila. Če na seznamu izberete sporočilo, se vrednost  **ID-ja**  sporočila prikaže v  **prikazanem podoknu**  s podrobnostmi. Skrbniki lahko s funkcijo [sledenja sporočilu](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) poiščejo sporočila in ustrezne vrednosti ID-ja sporočila.
- **E-poštni naslov pošiljatelja:** e-poštni naslov enega pošiljatelja.
- **E-poštni naslov** prejemnika: e-poštni naslov enega prejemnika.
- **Zadeva:** uporabite celotno zadevo sporočila. Iskanje ne uporablja velikih in malih črk.

Ko vnesete pogoje iskanja, kliknite Osveži gumb ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži, da** filtrirate rezultate.  

Ukazi »cmdlet« za ogled in upravljanje sporočil in datotek v karanteni so:
- [Brisanje-karantenamessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz v karanteno](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Predogled in pošiljanje sporočil v karanteni:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)ta ukaz »cmdlet« je le za sporočila in ne za datoteke z zlonamerno programsko opremo iz storitve ATP za SharePoint Online, OneDrive za podjetja ali Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)