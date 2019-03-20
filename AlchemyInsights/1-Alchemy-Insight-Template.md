---
title: enako kot ime datoteke je najboljši
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: ec979c2f2246fa06945b79bbb9348a7a57ad5180
ms.sourcegitcommit: b3cf5130ac8118f0fed66abe5286aa80ee91af52
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/19/2019
ms.locfileid: "30683865"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Zahteva alkimije glavo H1, H2 je ne dela.
Najboljše prakse in smernice za alkimijo authoring:

1. **Ne ugnezdite Alchemy vpogled v mapah**- to bo prekinil url strukture. Iščemo v pritrjevanje to.
1. Datoteke v mapi **AlchemyInsights** morajo imeti male črke imena datotek z vezaji za prostore ex. ***kako-to-usposobiti--čakanje***.
    1. Vključujejo ID pravilo ID ali vedro iz [alkimije Partner portal](https://alchemyportal.azurewebsites.net) na ms.custom področju. ex. ***MS.Custom: 100021***
1. Preostanek metapodatke na vrhu te datoteke uporabite kot predlogo.
1. [Alchemy Partner portal](https://alchemyportal.azurewebsites.net)pluti niz v oddelku **strank vpogled naslova:** in uporabo, ki kot začetno točko za vaš H1 naslov za vpogled. 
    > [!NOTE]
    > Alkimija vpogled mora imeti samo eno H1 na vrhu, ali bo prekinil v proizvodnji. H2s ne postanejo tako uporabo **krepko** ali drugih konvencij, da se označi ločenih odsekih.
1. Nato izpolnite telesa besedila z uporabo osnutek material v razdelku strank vpogled Alchemy pravilo strani
    1. Označeni seznami so v redu
    1. Tudi oštevilčene sezname
    1. **Krepko** in *Ležeče* so ok-
    1. Povezave morajo biti vedno bodisi **"povezave do spletnih" / zunanje** ali **globoko povezav z elementi uporabniškega vmesnika**, ni notranjih povezav.
    1. Slike ni uradno podprta v tem trenutku, vendar je na načrtu.

In to je res že malo predolgo. Najboljše prakse je približno 400 znakov---

Ko vsebino, je pripravljen, potegnem v živo veja. Potem obiščite [alkimije Partner portal](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje url. M