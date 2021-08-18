---
title: Preberite, kdo je nastavil posredovanje za nabiralnik, in kako
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
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317824"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Preberite, kdo je nastavil posredovanje za nabiralnik, in kako

Če je bilo zunanje posredovanje nastavljeno za nabiralnik, je dejavnost nadzorovana kot del ukaza »cmdlet« **Set-Mailbox.** Dejavnost v dnevniku nadzora najdete tako:

1. Naredite nekaj od tega:
   - V Središče za skladnost okolja Microsoft 365 <https://compliance.microsoft.com> pojdite na Nadzor  \> **rešitev.** Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://compliance.microsoft.com/auditlogsearch> .
   - V portalu Microsoft 365 Defender pojdite <https://security.microsoft.com> na **Nadzor**. Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://security.microsoft.com/auditlogsearch> .

   **Opomba:** Če opazite obvestilo, da morate vklopiti nadzor, ga vklopite zdaj. Če ta funkcija ni vklopljena, rezultati iskanja ne bodo mogli vleči podatkov iz prejšnjih datumov.

2. Na strani **Nadzor** preverite, ali je **izbran zavihek** Iskanje, nato pa konfigurirajte te nastavitve:
   - Izberite datumski/časovni obseg v **poljih** **Začetek** in Konec.
   - Preverite polje **Dejavnosti** vsebuje **Prikaz rezultatov za vse dejavnosti.**

3. Ko končate, kliknite **Iskanje.** Dejavnosti so prikazane na novi **strani Nadzora** iskanja.

4. V rezultatih kliknite stolpec Dejavnost, **da razvrstite** rezultate, in poiščite Nastavitve **nabiralnikov.**

5. V rezultatih izberite dejavnost, da odprete letak s podrobnostmi. Če želite ugotoviti, ali je dejavnost povezana s posredovanjem e-pošte, si morate ogledati podrobnosti vsakega zapisa nadzora:
   - **ObjectId**: Vrednost vzdevka nabiralnika, ki je bil spremenjen.
   - **Parametri:** _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.
   - **Id uporabnika:** Uporabnik, ki je konfiguriral posredovanje e-pošte za nabiralnik v polju **ObjectId.**

Če želite več informacij, glejte [Določanje, kdo je nastavil posredovanje e-pošte za nabiralnik.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
