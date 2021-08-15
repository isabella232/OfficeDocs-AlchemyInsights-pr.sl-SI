---
title: Odpravljanje napake »Aplikacije ni bilo mogoče odkriti«
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
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026130"
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
