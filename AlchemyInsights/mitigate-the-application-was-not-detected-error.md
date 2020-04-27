---
title: Odpravljanje napake »Aplikacije ni bilo mogoče odkriti«
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810499"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Odpravljanje napake »Aplikacije ni bilo mogoče odkriti«

Do napake pri namestitvi aplikacije, »Aplikacije ni bilo mogoče  odkriti po uspešno dokončani namestitvi,« ki se prikaže v programu Intune, lahko pride v vseh glavnih platformah OS (Windows, iOS in Android).

Najpogostejši scenariji, ki povzročijo to napako, vključujejo:

- Program je bil po začetni uvedbi posodobljen zunaj programa Intune (iz trgovine z aplikacijami tretjih oseb). Nekateri programi, na primer, kot je Google Chrome, lahko izvedejo samodejne posodobitve.
- Uporabnik je odstranil aplikacijo po prvotni namestitvi.

Če želite to težavo ublažiti, najprej opravite pregled prizadetih naprav, da določite scenarij, v katerem pride do napake.

- Če je bil program posodobljen zunaj programa Intune, je uvedba programa lahko nastavljena tako, da prezre različico aplikacije. To naredite tako, da v razdelku **Konfiguracija aplikacije > Informacije o aplikaciji** nastavite različico **Prezri aplikacijo** v **Da**.
- Pri ciljanju na stranko je morda primerno, da aplikacijo namestite kot je »zahtevano«, in tako zagotovite, da bo uvedena najnovejša različica.
- Druga možnost je, da v platformi iOS uporabite **funkcijo samodejnega posodabljanja**, ki je povezana s programom za količinski nakup Apple, ki ga lahko konfigurirate tako, da bo samodejno posodabljal nove različice aplikacij, ko bodo na voljo.

Če želite več informacij o odpravljanju težav z namestitvijo aplikacije, si oglejte [Odpravljanje težav z namestitvijo aplikacije](https://docs.microsoft.com/intune/troubleshoot-app-install).
