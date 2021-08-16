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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028769"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznavanje konfiguracije posredovanja zunanje e-pošte v nabiralnikih

Ko uporabnik Microsoft 365 zunanje posredovanje e-pošte v nabiralniku, je dejavnost nadzorovana kot del ukaza »cmdlet« **Set-Mailbox.** Dejavnost si lahko ogledate s funkcijo iskanja v dnevniku nadzora v središču & za skladnost s predpisi.

1. Prijavite se v središče [za Microsoft 365 s predpisi.](https://protection.office.com/)

2. Pojdite na stran **iskanja**  >  **v dnevniku nadzora** iskanja.

3. Izberite datumski obseg v **poljih Začetni datum** in **Končni** datum. Uporabniškega imena vam ni treba navesti. Preverite, **ali je** polje Dejavnosti nastavljeno na Prikaz rezultatov za vse **dejavnosti.**

4. Kliknite **Iskanje.**

V rezultatih kliknite **Filtriraj rezultate** in v polje filtra dejavnosti vnesite **Set-Mailbox.** V rezultatih izberite zapis nadzora. V **oknu** Podrobnosti kliknite **Več informacij.** Če želite ugotoviti, ali je dejavnost povezana s posredovanjem e-pošte, si morate ogledati podrobnosti vsakega zapisa nadzora.

- **ObjectId**: Vrednost vzdevka nabiralnika, ki je bil spremenjen.

- **Parametri:** _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.

- **Id uporabnika:** Uporabnik, ki je konfiguriral posredovanje e-pošte za nabiralnik v polju **ObjectId.**

Če želite več informacij, glejte [Določanje, kdo je nastavil posredovanje e-pošte za nabiralnik.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
