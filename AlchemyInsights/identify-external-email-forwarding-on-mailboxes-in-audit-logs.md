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
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752036"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Ko zunanje email odpošiljanje konfiguriran na nabiralnike

Ko uporabnik konfigurira posredovanje zunanji e-poštni nabiralnik, se nadzoruje dejavnosti kot del ukaza »cmdlet« **Set-Mailbox** . Si lahko ogledate uporabo revizijskih dnevnik iskanja v varnostno & Center skladnosti dejavnosti.

1. Prijavite se v [Office 365 varnost & skladnosti Center](https://protection.office.com/)

2. Kliknite **Išči ter preiskave** in izberite **Išči dnevnika nadzora**.

3. Izberite datumski obseg v polji **Začetni datum** in **končni datum** . Vam ni treba navesti uporabniško ime. Preverite, ali je polje **dejavnosti** nastavite pokazati **rezultate za vse dejavnosti**.

4. Kliknite **Išči**.

Na seznamu rezultatov kliknite **Filter rezultatov** in vnesite **Set-Mailbox** v precejalo škatla dejavnost. Izberite revizijski zapis v rezultatih. V pojavni meni **podrobnosti** , kliknite **več informacij**. Moraš pogledati podrobnosti o vsaki revizijski zapis ugotoviti, če je dejavnost povezana z email odpošiljanje.

- **ObjectId**: vrednost Vzdevek nabiralnika, ki je bila spremenjena.

- **Parametri**: _ForwardingSmtpAddress_ označuje ciljni e-poštni naslov.

- **ID uporabnika**: uporabnika, ki je konfiguriran posredovanje e-pošte v nabiralniku **ObjectId** področju.

Če želite več informacij, glejte [določanje ki nastaviti e-pošte, posredovanje za nabiralnik](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
