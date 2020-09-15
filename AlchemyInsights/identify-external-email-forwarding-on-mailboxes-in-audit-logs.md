---
title: Prepoznavanje zunanjega posredovanja e-pošte v nabiralnikih v dnevnikih nadzora
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696313"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Prepoznavanje, ko je zunanja e-poštna preusmeritev konfigurirana v nabiralnikih

Ko uporabnik programa Microsoft 365 konfigurira zunanjo posredovanje e-pošte v nabiralniku, je dejavnost revidirana kot del ukaza» cmdlet « **set-Mailbox** . V središču za skladnost varnosti & lahko vidite dejavnost z iskanjem dnevnika nadzora.

1. Prijavite se v središče za preverjanje [varnosti & za skladnost s predpisi Microsoft 365](https://protection.office.com/).

2. Pojdite na stran **Search**  >  **iskanje dnevnika nadzora** iskanja.

3. Izberite datumski obseg v poljih **Začetni datum** in **končni datum** . Ni vam treba določiti uporabniškega imena. Preverite, ali je polje **dejavnosti** nastavljeno tako, da **prikazuje rezultate za vse dejavnosti**.

4. Kliknite **Išči**.

V rezultatih kliknite **Filtriraj rezultate** in vnesite **nabiralnik** v polje Filter dejavnosti. V rezultatih Izberite zapis nadzora. V razdelku **podrobnosti** flyout kliknite **več informacij**. Če želite ugotoviti, ali je dejavnost povezana z odpošiljanjem e-pošte, si morate ogledati podrobnosti posameznega revizijskega zapisa.

- **Objectid**: vrednost vzdevka nabiralnika, ki je bil spremenjen.

- **Parametri**: _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.

- **ID**uporabnika: uporabnik, ki je konfiguriral posredovanje e-pošte v nabiralniku v polju» **objectid** «.

Če želite več informacij, glejte [določanje, kdo je nastavil posredovanje e-pošte za nabiralnik](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
