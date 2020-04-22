---
title: Prepoznavanje zunanjega posredovanja e-pošte v nabiralnikih v dnevnikih revizij
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716476"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ugotovite, kdaj je zunanje posredovanje e-pošte konfigurirano v nabiralnikih

Ko uporabnik Microsoft 365 konfigurira zunanje posredovanje e-pošte v nabiralniku, se dejavnost revidira kot del ukaza» cmdlet « **set-Mailbox** . Dejavnost lahko vidite s pomočjo iskanja dnevnika revizij v središču za skladnost varnostnega &.

1. Prijavite se v [Microsoft 365 Security & center za skladnost](https://protection.office.com/).

2. Pojdite na stran za**iskanje dnevnika revizij** **iskanja** > .

3. Izberite časovno območje v polji **Začetni datum** in **končni datum** . Uporabniškega imena ni treba določiti. Preverite, ali je polje **dejavnosti** nastavljeno tako, da **prikazuje rezultate za vse dejavnosti**.

4. Kliknite **Iskanje**.

V rezultatih kliknite **filter rezultati** in vrsta **set-poštni nabiralnik** v filter dejavnosti škatla. V rezultatih Izberite zapis o reviziji. V pojavnem meniju **podrobnosti** kliknite **več informacij**. Če želite ugotoviti, ali je dejavnost povezana s posredovanjem e-pošte, morate pogledati podrobnosti vsakega revizijskega zapisa.

- **Objectid**: vrednost vzdevka nabiralnika, ki je bil spremenjen.

- **Parametri**: _forwardingsmtpaddress_ označuje ciljni e-poštni naslov.

- **Userid**: uporabnik, ki je konfiguriral posredovanje e-pošte v nabiralniku v polju **objectid** .

Če želite več informacij, glejte [določanje, kdo je nastavil posredovanje e-pošte za nabiralnik](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
