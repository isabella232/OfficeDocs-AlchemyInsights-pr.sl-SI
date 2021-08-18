---
title: Branje dnevnikov nadzora za izbrisane dogodke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324749"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Branje dnevnikov nadzora za izbrisane dogodke

To naredite tako:

1. Naredite nekaj od tega:
   - V Središče za skladnost okolja Microsoft 365 na <https://compliance.microsoft.com> strani , pojdite na **Nadzor** \> **rešitev.** Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://compliance.microsoft.com/auditlogsearch> .
   - V portalu Microsoft 365 Defender na <https://security.microsoft.com> spletnem mestu , pojdite na **Nadzor**. Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://security.microsoft.com/auditlogsearch> .

    **Opomba:** Če opazite obvestilo, da morate funkcijo vklopiti, jo vklopite zdaj. Če funkcija ni vklopljena, rezultati iskanja ne bodo mogli vleči podatkov iz prejšnjih datumov.

2. Na **zavihku** Iskanje na **strani** Nadzor konfigurirajte te nastavitve:
   - **Datumski** in časovni obseg: Izberite datumski/časovni obseg v **poljih** **Začetek** in Konec.
   - **Dejavnosti:** vnesite **Exchange nabiralnika** in nato izberite te vrednosti:
     - **Izbrisana sporočila iz mape »Izbrisano«**
     - **Premaknjena sporočila v mapo »Izbrisano«**

       Ko končali, kliknite zunaj podokna, da minimizirate **podokno** Dejavnosti.

   - **Uporabniki:** Sprejmite prazno privzeto vrednost, če želite vrniti rezultate za vse uporabnike, ali pa vnesite enega ali več uporabnikov.

3. Ko končate, kliknite **Iskanje.** Dejavnosti so prikazane na novi **strani Nadzora** iskanja.

4. V rezultatih izberite dejavnost, da odprete letak s podrobnostmi. Dodatne informacije o izbrisanem elementu, na primer vrstica z zadevo in mesto elementa, ko je bil izbrisan, so prikazane v polju **AffectedItems.**

   **Opomba:** Izbrisanih elementov ne morete obnoviti s funkcijo dnevnika nadzora. Če želite obnoviti izbrisane elemente, glejte [Obnovitev izbrisanih e-poštnih sporočil Outlook v spletu](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11).

Če želite več informacij, glejte [Iskanje po dnevniku nadzora in preiskovanje pogostih težav s podporo.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
