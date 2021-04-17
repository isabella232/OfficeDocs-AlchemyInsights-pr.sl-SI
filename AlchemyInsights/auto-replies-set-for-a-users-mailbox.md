---
title: Nastavite samodejne odgovore za nabiralnik
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820950"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Nastavite samodejne odgovore za nabiralnik uporabnika

**Način 1**

1. Vpišite se v portal Microsoft 365.

2. Izberite **Uporabniki > Aktivni uporabniki** (ali **Skupine > Nabiralniki v skupni rabi**, če to nastavljate za nabiralnik v skupni rabi).

3. Izberite uporabnika, ki ima Microsoft Exchangeev nabiralnik.

4. V pojavnem meniju na desni izberite **Nastavitve pošte > Samodejni odgovori** (če gre za nabiralnik v skupni rabi, v pojavnem obvestilu preprosto kliknite **Samodejni odgovori**).

**Način 2**

1. Vpišite se v skrbniški portal okolja Microsoft 365 s skrbniškimi poverilnicami.

2. Razširite razdelek **Skrbniška središča** in kliknite **Exchange**.

3. Kliknite sliko v zgornjem desnem kotu, kliknite **Drug uporabnik**, nato pa izberite uporabniški nabiralnik, ki ga želite spremeniti.

4. Na levi strani izberite **Možnosti**, kliknite **Organiziraj e-pošto**, nato pa kliknite **Samodejni odgovori.**

**Način 3**

Zaženite ta pripomoček »cmdlet« v storitvi Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Če želite več informacij o tem pripomočku »cmdlet«, glejte [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
