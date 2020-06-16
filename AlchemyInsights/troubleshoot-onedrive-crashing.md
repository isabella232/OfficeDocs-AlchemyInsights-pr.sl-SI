---
title: Odpravljanje težav s storitvijo OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749169"
---
# <a name="troubleshoot-onedrive-crashes"></a>Odpravljanje težav s storitvijo OneDrive

Če se storitev OneDrive večkrat zruši, poskusite te korake za odpravljanje težav:

**Zagotovite, da registrski ključi niso določeni:**

1. Z urejevalnikom registra krmarite do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Če DisableFileSyncNGSC je sedanji ter število enakih oseb v 1, plan zakleniti ter sprememba vrednost v 0.
3. Ročno zaženite OneDrive, tako da se bo začela ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), v iskalno polje vnesite OneDrive in kliknite na namizno aplikacijo OneDrive.

**Ponastavi OneDrive:**

Opombe:

- Ponastavitev storitve OneDrive prekine povezavo vseh obstoječih sinhronizacijskih povezav (vključno z vašo osebno storitvijo OneDrive, če je nastavljena).
- Datotek ali podatkov ne boste izgubili tako, da ponastavite OneDrive v računalniku.

**Če želite ponastaviti OneDrive:**

1. Odprite pogovorno okno Zaženi tako, da pritisnete tipko Windows in R.
2. Vnesite% localappdata% \Microsoft\OneDrive\onedrive.exe/Ponastavi in pritisnite OK. Na kratko se lahko prikaže okno ukaznega okna.
3. Ročno zaženite OneDrive, tako da se bo začela ![Pritisnite tipko Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), v iskalno polje vnesite OneDrive in kliknite na namizno aplikacijo OneDrive.

Opombe:

- Če ste se odločili za sinhronizacijo le nekaj map pred ponastavitvijo, boste morali to storiti znova, ko je končana sinhronizacija. Če želite več informacij, preberite [Izberite, katere mape v storitvi OneDrive želite sinhronizirati z računalnikom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- To boste morali dokončati za osebne storitve OneDrive in OneDrive za podjetja.