---
title: Iskanje dogodkov, ki se izvajajo v pravilih za mapo »Prejeto«
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313515"
---
# <a name="find-events-performed-on-inbox-rules"></a>Iskanje dogodkov, ki se izvajajo v pravilih za mapo »Prejeto«

Ko ustvarite, spremenite ali izbrišete pravila za mapo »Prejeto«, se dogodki beležijo v dnevnik nadzora. Oglejte si jih tako:

1. Naredite nekaj od tega:
   - V Središče za skladnost okolja Microsoft 365 na <https://compliance.microsoft.com> strani , pojdite na **Nadzor** \> **rešitev.** Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://compliance.microsoft.com/auditlogsearch> .
   - V portalu Microsoft 365 Defender na <https://security.microsoft.com> spletnem mestu , pojdite na **Nadzor**. Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://security.microsoft.com/auditlogsearch> .

    **Opomba:** Če opazite obvestilo, da morate vklopiti nadzor, ga vklopite zdaj. Če ta funkcija ni vklopljena, rezultati iskanja ne bodo mogli vleči podatkov iz prejšnjih datumov.
1. Izberite polje Dejavnosti in poiščite Exchange nabiralnika, nato pa izberite New-InboxRule pravila za mapo »Prejeto« Outlook spletnem programu. Ko končali, kliknite zunaj podokna, da minimizirate podokno Dejavnosti.
1. Določite datumski obseg in nato v polju Uporabniki izberite uporabniško ime uporabnika, ki ga želite raziskati. Izberete lahko več uporabnikov hkrati.
1. Izberite Išči. Dejavnosti so prikazane v razdelku Rezultati.
1. Če si želite ogledati podrobnosti, izberite dejavnost, nato pa izberite Več informacij. V razdelku Parametri si lahko ogledate ime pravila, nabor pogojev in dejanja, ki jih bo pravilo izvnelo.

2. Na **zavihku** Iskanje na **strani** Nadzor konfigurirajte te nastavitve:
   - **Datumski** in časovni obseg: Izberite datumski/časovni obseg v **poljih** **Začetek** in Konec.
   - **Dejavnosti:** Izberite **Novo-PrejetoPravi pravilo za ustvarjanje mape »Prejeto« Outlook spletnem programu**

3. Ko končate, kliknite **Iskanje.** Dejavnosti so prikazane na novi **strani Nadzora** iskanja.

4. V rezultatih izberite dejavnost, da odprete letak s podrobnostmi. V **razdelku Parametri** si lahko ogledate ime pravila, nabor pogojev in dejanja, ki jih bo pravilo izvnelo.

Če želite izvedeti več, glejte [Iskanje po dnevniku nadzora in raziskovanje pogostih težav s podporo.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
