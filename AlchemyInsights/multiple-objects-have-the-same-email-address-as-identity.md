---
title: Več predmetov ima enak e-poštni naslov kot identiteta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439710"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Več predmetov ima enak e-poštni naslov kot identiteta

**Več predmetov**

Eden od pogostih razlogov za to napako je, da ne more pravilno usmerjati zahteve outlookovega spletnega dostopa v prisotnosti več predmetov z istim e-poštnim naslovom kot identiteta. Če želite poiskati te predmete, zaženite te ukaze:

· Prejemnika<email address>

· Pridobitev uporabnika<email address>

· Pridobitev <email address> uporabnika -SoftDeletedUser

· Pokliči stik<email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Nabiralnik <email address> -IncludeSoftDeletedMailbox

· Get-Poštni <email address> nabiralnik -NeaktivnoMailboxOnly

Če želite odpraviti težavo, odstranite več predmetov z isto e-poštno identiteto in se prepričajte, da obstaja en predmet z določeno e-poštno identiteto in da je njena vrsta prejemnika UserMailbox.

**Isti naslov se uporablja za poslovne in potrošniške nabiralnike**

Drug vzrok je, ko se isti naslov uporablja za poslovne in potrošniške nabiralnike. v to skrinja, uporabnik morati sprememba svoj primaren potrošnik alias do kavarna zaslomba to lliterarna podlaga dramskega dela. To je trajna napaka, ki ne izgine brez posredovanja.

Če želite podrobnosti, [glejte Spreminjanje e-poštnega naslova ali telefonske številke za Microsoftov račun](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).