---
title: Podvojitev zapisov naprav v portalu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2020
ms.locfileid: "43790173"
---
# <a name="duplicate-device-record-in-the-portal"></a>Podvojitev zapisov naprav v portalu

V portalu boste morda videli 2 zapisa za napravo, če naprava spletnemu mestu upravitelja konfiguracije trenutno ne poroča stanja soupravljanja. Če želite preveriti stanje soupravljanja naprave, si oglejte stolpec **Soupravljano** za napravo v konzoli upravitelja konfiguracije. Če stolpec ni viden, ga lahko dodate tako, da z desno tipko miške kliknite glave stolpcev in ga izberete na seznamu.

Vrednost soupravljanja mora biti **Da**. Če je vrednost **Ne**, odprite aplikacijo odjemalca upravitelja konfiguracije v odjemalski napravi in preverite vrednost lastnosti **Soupravljanje** na zavihku »Splošno«.

- Če je vrednost **Omogočeno**, kaže to na težave pri komunikaciji odjemalca s točko upravljanja. Če želite poiskati morebitne težave s povezljivostjo, preglejte dnevnik **CcmMessaging.log** v napravi.

- Če je vrednost **Onemogočeno**, naprava pa je včlanjena v Intune, preverite, ali je naprava prejela pravilnik o soupravljanju. To naredite tako, da v napravi pregledate dnevnik **CoManagementHandler.log**.
