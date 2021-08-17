---
title: enako kot je ime datoteke najboljša
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312841"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>»Zahtevano Alchemy Glava H1, H2 ne deluje.«
Najboljše prakse in smernice za avtorje Alchemy:

1. **Ne ugnezdite datoteke Alchemy Vpogledi mape**– s tem boste prekinili strukturo url-ja. To težavo se želimo popraviti.
1. Datoteke v mapi **AlchemyInsights** morajo imeti imena datotek z malimi črkami z vezaji za presledke ex. **_how-to-enable-litigation-hold_**.
    1. ID pravila ali ID vedra vključite v [partnerski portal Alchemy](https://alchemyportal.azurewebsites.net) v polje ms.custom. ex. ***ms.custom: 100021***
1. Uporabite preostale metapodatke na vrhu te datoteke kot predlogo.
1. Na [portalu za partnerje Alchemy](https://alchemyportal.azurewebsites.net)se pomaknite navzdol do razdelka **Customer Insight Title:** (Naslov vpogleda stranke): nato pa to uporabite kot izhodišče za svoj naslov H1 za vpogled. 

**Opomba:** Alchemy Vpogledi MORAJO imeti le en H1 na vrhu, drugače se prelomijo v produkciji. H2s ne bodo upodobiti, zato za podpisovanje ločenih odsekov uporabite krepko pisavo ali druge dogovore. 
1. Nato izpolnite telo besedila z materialom za osnutek v Customer Insights na strani pravila Alchemy
    1. Označeni seznami so v redu
    1. Tudi oštevilčeni seznami
    1. **Krepko** *in ležeče je* vse v redu
    1. Povezave morajo biti vedno **»povezave do spleta«/zunanje** ALI globoke povezave do elementov **uporabniškega** vmesnika, ne pa notranjih povezav.
    1. Slike trenutno niso uradno podprte, vendar so v načrtu.

To je pravzaprav že predolga. Najboljša praksa je približno 400 ---------------------------------

Ko je vsebina pripravljena, jo povlecite v vejo v živo. Nato pojdite na portal [za partnerje Alchemy](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje url. 