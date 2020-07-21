---
title: Uporabnik prejme napako AADSTS7000112 Yammer je onemogočen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198371"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Uporabnik prejme napako AADSTS7000112 Yammer je onemogočen

Če se prikaže napaka "AADSTS7000112: aplikacija" 00000005-0000-0ff1-CE00-000000000000 "(Yammer) je onemogočena", obstaja težava pri ravnatelju storitve v storitvi Azure AD. Skrbnik je morda onemogočil naročitelja storitev, da blokira dostop do storitve Yammer.

Onemogočanje glavnega servisa ni priporočeno in lahko povzroči dodatna vprašanja. Če želite več informacij o podprtem pristopu za blokiranje uporabniškega dostopa do programa Yammer, glejte izklop [dostopa do storitev yammer za Microsoftove uporabnike 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Če želite to težavo odpraviti v portalu Azure in obnoviti dostop uporabnikov do storitev Yammer:

1.  Odprite stran Azure Active Directory in izberite **aplikacije podjetja** pod **Upravljaj** v levem podoknu za krmarjenje.
3.  V iskalno polje vnesite **Office 365 Yammer** in izberite ime aplikacije, da odprete nastavitve.
4.  V levem podoknu za krmarjenje izberite **lastnosti** pod **Upravljaj** .
5.  Nastavite vrednost **omogočenega za prijavo za uporabnike?** za **Yes**in nato izberite **Shrani**.
6.  Znova se vpišite v Yammer. Morda boste morali počistiti piškotke.

Izmeničen, prost dostop PowerShell zapoved v število enakih oseb vrednost. Če želite več informacij, glejte ["Žal mi je, vendar imamo težave pri vpisu v" napako, ko kliknete ploščico Yammer v Officeu 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 