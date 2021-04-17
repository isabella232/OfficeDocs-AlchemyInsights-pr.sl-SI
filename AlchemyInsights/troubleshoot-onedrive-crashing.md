---
title: Odpravljanje težav z zrušitve storitve OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826215"
---
# <a name="troubleshoot-onedrive-crashes"></a>Odpravljanje težav z zrušitve storitve OneDrive

Če se OneDrive večkrat zruši, poskusite to:

**Zagotovite, da registrski ključi niso nastavljeni:**

1. Z urejevalnikom registra odprite HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Če je DisableFileSyncNGSC prisoten in nastavljen na 1, odprite ključ in spremenite vrednost na 0.
3. Ročni zagon storitve OneDrive v začetnem meniju ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), v iskalno polje vnesite OneDrive in kliknite namizno aplikacijo OneDrive.

**Ponastavite OneDrive:**

Opombe:

- S ponastavitvijo storitve OneDrive boste prekinili vse obstoječe povezave za sinhronizacijo (tudi osebni OneDrive, če je nastavljen).
- S ponastavitvijo storitve OneDrive v računalniku ne boste izgubili datotek ali podatkov.

**Če želite ponastaviti OneDrive:**

1. Odprite pogovorno okno »Zaženi« tako, da pritisnete tipko Windows in R.
2. Vnesite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset in pritisnite V redu. Za kratek čas se lahko prikaže ukazno okno.
3. Ročni zagon storitve OneDrive v začetnem meniju ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), v iskalno polje vnesite OneDrive in kliknite namizno aplikacijo OneDrive.

Opombe:

- Če ste se odločili, da pred ponastavitvijo sinhronizirate le nekatere mape, boste morali to storiti znova, ko bo sinhronizacija končana. Če [želite več informacij, preberite Izberite mape storitve OneDrive, ki jih želite sinhronizirati](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   z računalnikom.
- To boste morali dokončati za osebni OneDrive in OneDrive za podjetja.