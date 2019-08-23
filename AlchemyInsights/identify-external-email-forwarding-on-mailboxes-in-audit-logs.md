---
title: Prepoznavanje posredovanje zunanji e-poštni nabiralniki v dnevnikih nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539117"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ko zunanje email odpošiljanje konfiguriran na nabiralnike

Ko Office 365 uporabnik konfigurira posredovanje zunanji e-poštni nabiralnik, se nadzoruje dejavnosti kot del ukaza »cmdlet« **Set-Mailbox** . Si lahko ogledate uporabo revizijskih dnevnik iskanja v varnostno & Center skladnosti dejavnosti.

1. Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/).

2. Pojdi na **Iskanje** > **revizije dnevnik iskalna** stran.

3. Izberite datumski obseg v polji **Začetni datum** in **končni datum** . Vam ni treba navesti uporabniško ime. Preverite, ali je polje **dejavnosti** nastavite pokazati **rezultate za vse dejavnosti**.

4. Kliknite **Išči**.

Na seznamu rezultatov kliknite **Filter rezultatov** in vnesite **Set-Mailbox** v precejalo škatla dejavnost. Izberite revizijski zapis v rezultatih. V pojavni meni **podrobnosti** , kliknite **več informacij**. Moraš pogledati podrobnosti o vsaki revizijski zapis ugotoviti, če je dejavnost povezana z email odpošiljanje.

- **ObjectId**: vrednost Vzdevek nabiralnika, ki je bila spremenjena.

- **Parametri**: _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.

- **ID uporabnika**: uporabnika, ki je konfiguriran posredovanje e-pošte v nabiralniku **ObjectId** področju.

Če želite več informacij, glejte [določanje ki nastaviti e-pošte, posredovanje za nabiralnik](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
