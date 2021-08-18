---
title: Prepoznavanje posredovanja zunanje e-pošte v nabiralnikih v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899900"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznavanje konfiguracije posredovanja zunanje e-pošte v nabiralnikih

Ko uporabnik Microsoft 365 zunanje posredovanje e-pošte v nabiralniku, je dejavnost nadzorovana kot del ukaza »cmdlet« **Set-Mailbox.** Dejavnost si lahko ogledate z iskanjem v dnevniku nadzora. To naredite tako.

1. Naredite nekaj od tega:
   - V Središče za skladnost okolja Microsoft 365 pojdite <https://compliance.microsoft.com> na Nadzor  \> **rešitev.** Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://compliance.microsoft.com/auditlogsearch> .
   - V portalu Microsoft 365 Defender na <https://security.microsoft.com> spletnem mestu , pojdite na **Nadzor**. Če pa se želite neposredno po vrniti na **stran Nadzor,** uporabite <https://sip.security.microsoft.com/auditlogsearch> .

2. Na strani **Nadzor** preverite, ali je **izbran zavihek** Iskanje, nato pa konfigurirajte te nastavitve:
   - Izberite datumski/časovni obseg v **poljih** **Začetek** in Konec.
   - Preverite polje **Dejavnosti** vsebuje **Prikaz rezultatov za vse dejavnosti.**

3. Ko končate, kliknite **Iskanje.** Dejavnosti so prikazane na novi **strani Nadzora** iskanja.

4. V rezultatih kliknite **Filtriraj rezultate** in v polje filtra dejavnosti vnesite **Set-Mailbox.**

5. V rezultatih izberite zapis nadzora. V **oknu** Podrobnosti kliknite **Več informacij.** Če želite ugotoviti, ali je dejavnost povezana s posredovanjem e-pošte, si morate ogledati podrobnosti vsakega zapisa nadzora.

   - **ObjectId**: Vrednost vzdevka nabiralnika, ki je bil spremenjen.
   - **Parametri:** _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.
   - **Id uporabnika:** Uporabnik, ki je konfiguriral posredovanje e-pošte za nabiralnik v polju **ObjectId.**

Če želite več informacij, glejte [Določanje, kdo je nastavil posredovanje e-pošte za nabiralnik.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
