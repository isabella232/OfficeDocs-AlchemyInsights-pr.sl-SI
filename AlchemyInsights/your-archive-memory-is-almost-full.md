---
title: Nabiralnik arhiva je skoraj poln
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046768"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Nabiralnik arhiva je skoraj poln

Če uporabnik prejme opozorilo; **Nabiralnik arhiva je skoraj poln** ali pa morate povečati velikost nabiralnika arhiva, na voljo pa so ti namigi:

1. Če je uporabniku dodeljena licenca za Exchange Online (paket 1), nadgradite na **Exchange Online paket 2,** da povečate velikost s 50 GB na 100 GB.
1. Če je uporabniku že dodeljena nekaj od tega: Exchange Online (paket **2)** ali Exchange Online (paket 1) z dodatkom za Arhiviranje Exchange Online, sledite spodnjim korakom, da omogočite samodejno razširitev arhiviranja:
 
    1. [Povezovalnik, da Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Zaženite ta ukaz »commandlet« za uporabnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Zaženite ta ukaz »commandlet« in preverite, ali je omogočen za uporabnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Če želite več informacij, glejte:

- [Omogočanje neomejenega arhiviranja – pomoč za skrbnike – Microsoft 365 s predpisi | Microsoftovi dokumenti](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online omejitve – opisi storitve | Microsoftovi dokumenti](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nadgradnja na drug paket za | Microsoftovi dokumenti](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

