---
title: Nastavite samodejne odgovore za nabiralnik
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788898"
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
