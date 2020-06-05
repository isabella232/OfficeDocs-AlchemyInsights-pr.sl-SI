---
title: Manjkajoče e-pošte v karanteni
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569560"
---
# <a name="missing-emails-in-quarantine"></a>Manjkajoče e-pošte v karanteni "

Skrbniki [si lahko ta sporočila ogledajo, sprostijo ali izbrišejo.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Če želite odpreti središče za skladnost varnostnega &, pojdite na [https://protection.office.com](https://protection.office.com/) . Če želite neposredno odpreti stran» karantena «, pojdite na [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Iščete lahko po naslednjih vrednostih:  

- **ID sporočila**: globalni enolični identifikator sporočila. Če na seznamu izberete sporočilo, se vrednost ID- **ja sporočila** prikaže v podoknu za Pojavni meni **podrobnosti** , ki se prikaže. Skrbniki lahko s [sledenjem sporočilom](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) najdejo sporočila in ustrezne vrednosti ID-ja sporočila.
- **E-poštni naslov pošiljatelja**: e-poštni naslov enega pošiljatelja.
- **E-poštni naslov prejemnika**: e-poštni naslov enega prejemnika.
- **Zadeva**: uporabite celoten predmet sporočila. Iskanje ni občutljivo na male črke.

Ko vnesete kriterije iskanja, kliknite Osveži ![ gumb ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži** , da filtrirate rezultate.  

Ukazi» cmdlet «, ki jih uporabljate za ogled in upravljanje sporočil in datotek v karanteni, so:
- [Izbriši-karantenski sporočilo](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Sporočilo za izvoz-karanteno](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Sporočilo v karanteni](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Predogled-v karanteni](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Upoštevajte, da je ta ukaz» cmdlet «samo za sporočila, ne pa zlonamerna datoteka iz ATP za SharePoint online, OneDrive za podjetja ali ekipe.
- [Sporočilo za sprostitev-karanteno](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)