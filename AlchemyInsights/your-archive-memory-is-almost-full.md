---
title: Nabiralnik v arhivu je skoraj poln
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974664"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Nabiralnik v arhivu je skoraj poln

Če uporabnik prejme opozorilo; **Nabiralnik arhiva je skoraj poln** ali pa morate povečati velikost nabiralnika arhiva, tukaj je nekaj namigov:

1. Če je uporabniku dodeljen paket Exchange Online, nadgradite na licenco **Exchange Online za paket 2** , da povečate velikost od 50 GB do 100GB.
1. Če je uporabnik že dodelil nekaj od tega: **Exchange Online (paket 2** ) ali Exchange Online (paket 1) z dodatkom za arhiviranje v storitvi Exchange Online, uporabite spodnje korake, da omogočite samodejno razširjanje arhiviranja:.
 
    1. [Vzpostavite povezavo s storitvijo PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Zaženite te unifiedgroup za uporabnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Zaženite te unifiedgroup za potrditev, da je omogočena za uporabnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Če želite več informacij, glejte:

- [ Omogočanje neomejenega arhiviranja – pomoč za skrbnike – skladnost s predpisi Microsoft 365 | Microsoft docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Omejitve za Exchange Online – opisi storitev | Microsoft docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nadgradnja na drug poslovni načrt | Microsoft docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

