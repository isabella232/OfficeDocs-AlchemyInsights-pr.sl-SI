---
title: Raziščite vse dejavnosti uporabnikov
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: d05c8f02efc3bb92865880ea4a2338abaf7d70254f0b4bbfb566423e62b391dd
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898812"
---
# <a name="investigate-all-the-users-activities"></a>Raziščite vse dejavnosti uporabnikov

To naredite tako:

1. Naredite nekaj od tega:
   - V Središče za skladnost okolja Microsoft 365 na <https://compliance.microsoft.com> strani , pojdite na **Nadzor** \> **rešitev.** Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://compliance.microsoft.com/auditlogsearch> .
   - V portalu Microsoft 365 Defender na <https://security.microsoft.com> spletnem mestu , pojdite na **Nadzor**. Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Če opazite obvestilo, da morate funkcijo vklopiti, jo vklopite zdaj. Če funkcija ni vklopljena, rezultati iskanja ne bodo mogli vleči podatkov iz prejšnjih datumov.

2. Na **zavihku** Iskanje na **strani** Nadzor konfigurirajte te nastavitve:
   - **Datumski** in časovni obseg: Izberite datumski/časovni obseg v **poljih** **Začetek** in Konec.
   - **Dejavnosti:** Če vas zanima določena dejavnost, jo izberite na seznamu. sicer privzeta vrednost **Pokaži rezultate za vse dejavnosti vrne** vse dejavnosti.
   - **Uporabniki:** Sprejmite prazno privzeto vrednost, če želite vrniti rezultate za vse uporabnike, ali pa vnesite enega ali več uporabnikov.

3. Ko končate, kliknite **Iskanje.** Dejavnosti so prikazane na novi **strani Nadzora** iskanja. Videli boste naslov **IP,** **uporabnika** in **ime** dejavnosti.

4. Če želite prenesti  rezultate, izberite \> **Izvozi prenesi vse rezultate**.

5. V rezultatih izberite dejavnost, da odprete letak s podrobnostmi.

Če želite izvedeti več, glejte [Iskanje po dnevniku nadzora in raziskovanje pogostih težav s podporo.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
