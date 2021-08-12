---
title: Odpravljanje težav OneDrive sesutja
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
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921023"
---
# <a name="troubleshoot-onedrive-crashes"></a>Odpravljanje težav OneDrive sesutja

Če OneDrive večkrat zruši, poskusite to:

**Zagotovite, da registrski ključi niso nastavljeni:**

1. Z urejevalnikom registra odprite HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Če je DisableFileSyncNGSC prisoten in nastavljen na 1, odprite ključ in spremenite vrednost na 0.
3. Ročno zaženite OneDrive tako, da zaženete začetni meni ![Pritisnite tipko Windows tipko](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), vnesite OneDrive v iskalno polje in nato kliknite ikono OneDrive računalnika.

**Ponastavitev OneDrive:**

Opombe:

- S ponastavitvijo OneDrive prekinete povezave z vsemi obstoječimi povezavami za sinhronizacijo (vključno z osebnimi povezavami OneDrive če je nastavljena).
- Če ponastavite podatkovne datoteke ali podatke, jih OneDrive v računalniku.

**Ponastavitev OneDrive:**

1. Pogovorno okno Zaženi odprete tako, da pritisnete tipko Windows in R.
2. Vnesite %localappdata%\Microsoft\OneDrive\onedrive.exe /reset in pritisnite V redu. Za kratek čas se lahko prikaže ukazno okno.
3. Ročno zaženite OneDrive tako, da zaženete začetni meni ![Pritisnite tipko Windows tipko](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), vnesite OneDrive v iskalno polje in nato kliknite ikono OneDrive računalnika.

Opombe:

- Če ste se odločili, da pred ponastavitvijo sinhronizirate le nekatere mape, boste morali to storiti znova, ko bo sinhronizacija končana. Več [informacij najdete v OneDrive mapah za sinhronizacijo z](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   računalnikom.
- To boste morali dokončati za osebne OneDrive in OneDrive za podjetja.