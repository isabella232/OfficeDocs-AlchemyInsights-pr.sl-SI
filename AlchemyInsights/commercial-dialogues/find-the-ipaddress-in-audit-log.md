---
title: Iskanje naslova IP v dnevniku nadzora
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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303593"
---
# <a name="find-the-ip-address-in-audit-log"></a>Iskanje naslova IP v dnevniku nadzora

Naslov IP, ki ustreza dejavnosti, ki jo je izvedel uporabnik ali skrbnik, je prikazan v dnevnikih nadzora. Zabeležene so tudi informacije o odjemalcu. Naslov IP prepoznate tako:

1. Naredite nekaj od tega:
   - V Središče za skladnost okolja Microsoft 365 <https://compliance.microsoft.com> pojdite na Nadzor  \> **rešitev.** Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://compliance.microsoft.com/auditlogsearch> .
   - V portalu Microsoft 365 Defender na <https://security.microsoft.com> spletnem mestu , pojdite na **Nadzor**. Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://security.microsoft.com/auditlogsearch> .

    **Opomba:** Če opazite obvestilo, da morate vklopiti nadzor, ga vklopite zdaj. Če ta funkcija ni omogočena, rezultati iskanja ne bodo mogli vleči podatkov iz prejšnjih datumov.

2. Na strani **Nadzor** preverite, ali je **izbran zavihek** Iskanje, nato pa konfigurirajte te nastavitve:
   - **Datumski** in časovni obseg: Izberite datumski/časovni obseg v **poljih** **Začetek** in Konec.
   - **Dejavnosti:** Če vas zanima določena dejavnost, jo izberite na seznamu. v nasprotnem primeru vrne **privzeta vrednost Rezultate za** vse dejavnosti pokaži tako, da vrne vse dejavnosti. Upoštevajte, da določene dejavnosti morda niso na voljo za izbiro; vendar pa bodo ti elementi nadzora vrnjeni, **če je izbrana možnost Pokaži rezultate** za vse dejavnosti.
   - **Uporabniki:** Sprejmite prazno privzeto vrednost, če želite vrniti rezultate za vse uporabnike, ali pa vnesite enega ali več uporabnikov.

3. Ko končate, kliknite **Iskanje.** Dejavnosti so prikazane na novi **strani Nadzora** iskanja.

4. V rezultatih kliknite **Filtriraj rezultate** in v polje filtra dejavnosti vnesite **Set-Mailbox.**

5. V rezultatih izberite zapis nadzora, da odprete **letak** Podrobnosti.

Če želite več informacij, glejte [Iskanje po dnevniku nadzora in preiskovanje pogostih težav s podporo.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
