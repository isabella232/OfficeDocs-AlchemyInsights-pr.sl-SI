---
title: Odpravljanje težav z OneDrive zruši
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665014"
---
# <a name="troubleshoot-onedrive-crashes"></a>Odpravljanje težav z OneDrive zruši

Če se OneDrive večkrat zruši, poskusite s temi koraki za odpravljanje težav:

**Zagotovite, da registrski ključi niso nastavljeni:**

1. Uporaba urejevalnika registra se pomaknite do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Če je argument» DisableFileSyncNGSC «prisoten in nastavljen na 1, odprite tipko in spremenite vrednost na 0.
3. Ročno zaženite OneDrive tako, da začnete ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), v iskalno polje vnesite OneDrive in nato kliknite OneDrive namizni program.

**Ponastavi OneDrive:**

Opombe

- S ponastavitvijo OneDrive prekinete povezavo vseh obstoječih sinhronizacijskih povezav (vključno z vašim osebnim OneDrive, če ste nastavili).
- Datotek ali podatkov ne boste izgubili s ponastavitvijo OneDrive v računalniku.

**Če želite ponastaviti OneDrive:**

1. Odprite pogovorno okno za zagon tako, da pritisnete tipko Windows in R.
2. Vnesite% localappdata% \Microsoft\OneDrive\onedrive.exe/reset in pritisnite v redu. Ukazno okno se lahko prikaže na kratko.
3. Ročno zaženite OneDrive tako, da začnete ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), v iskalno polje vnesite OneDrive in nato kliknite OneDrive namizni program.

Opombe

- Če ste izbrali sinhronizacijo le nekaterih map pred ponastavitvijo, boste morali to narediti znova, ko bo sinhronizacija dokončana. Če želite več informacij, preberite [izbiranje, katere OneDrive mape želite sinhronizirati z računalnikom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- To boste morali dokončati za osebne OneDrive in OneDrive za podjetja.