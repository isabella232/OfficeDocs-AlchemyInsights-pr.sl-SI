---
title: 'enako kot ime datoteke, je najbolje [pravilo #-opis]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634520"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Zahteva alkimije glavo H1, H2 je ne dela.
Najboljše prakse in smernice za alkimijo authoring:

1. **Ne ugnezdite Alchemy vpogled v mapah**- to bo prekinil url strukture. Iščemo v pritrjevanje to.
1. Datoteke v mapi **AlchemyInsights** mora imeti pravilo ID in ime pravila iz [alkimije Partner portal](https://alchemyportal.azurewebsites.net) v ime datoteke.
    1. ex. ***976-how-to-enable-Litigation-Hold***
1. Metapodatke na vrhu te datoteke uporabite kot predlogo. Nič drugega ni potrebno.
1. [Alchemy Partner portal](https://alchemyportal.azurewebsites.net)pluti niz v oddelku **strank vpogled naslova:** in uporabo, ki kot začetno točko za vaš H1 naslov za vpogled. 
    > [!NOTE]
    > Alkimija vpogled mora imeti samo eno H1 na vrhu, ali bo prekinil v proizvodnji. H2s ne postanejo tako uporabo **krepko** ali drugih konvencij, da se označi ločenih odsekih.
1. Nato izpolnite telesa besedila z uporabo osnutek material v razdelku strank vpogled Alchemy pravilo strani
    1. Označeni seznami so v redu
    1. Tudi oštevilčene sezname
    1. **Krepko** in *Ležeče* so ok-
    1. Povezave morajo biti vedno bodisi **"povezave do spletnih" / zunanje** ali **globoko povezav z elementi uporabniškega vmesnika**, ni notranjih povezav.

In to je res že malo predolgo. Najboljše prakse je približno 400 znakov---

Ko vsebino, je pripravljen, potegnem v živo veja. Potem obiščite [alkimije Partner portal](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje url. Preverite, ali vpogled pregledali in objavila pravi, "da" in kliknite posodobitev pravilo. **(To bo videti lepši v novi različici portala - sproščanje soon.)** 
 ![url polje](media/for-content-team.PNG)

