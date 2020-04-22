---
title: isto kot filename je najprimernejši
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: e2dcca1295e37007593b34c2d818ad1d1133e4a1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676549"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>Zahtevana Alchemy header H1, H2's ne dela.
Najboljše prakse in smernice za authoring Alchemy:

1. **Ne gnezdijo Alchemy Insights v mapah**-to bo prekinil URL strukturo. Iščemo to.
1. Datoteke v mapi **Alchemyinsights** morajo imeti male imena datotek z vezaji za presledke ex. ***kako-v-usposobiti-pravda-počakaj***.
    1. Vključite ID pravila ali ID vedra iz [portala Alchemy partner](https://alchemyportal.azurewebsites.net) v polje po meri MS. Ex. ***MS. Custom: 100021***
1. Uporabite preostale metapodatke na vrhu te datoteke kot predlogo.
1. Na [portalu Alchemy partner](https://alchemyportal.azurewebsites.net), pomaknite navzdol do oddelka **Customer vpogled naslov:** in uporabite, da kot izhodišče za vaše h1 naslov za vpogled. 
    > [!NOTE]
    > Alchemy Insights mora imeti samo en H1 na vrhu ali pa bo prekinil v proizvodnji. H2s ne postanejo tako uporabljajo **krepko** ali druge konvencije, da pomeni ločene oddelke.
1. Nato izpolnite besedilo telesa z uporabo osnutka gradiva v razdelku vpogled v stranke na strani pravila Alchemy
    1. Označeni seznami so v redu
    1. Oštevilčeni seznami preveč
    1. **Krepko** in *Ležeče* so-ok
    1. Povezave morajo biti vedno bodisi **"povezave do spleta"/zunanje** ali **Deep-povezave do elementov UI**, ne notranjih povezav.
    1. Slike niso uradno podprte v tem trenutku, vendar je na časovnem načrtu.

In to je že malo predolgo. Najboljša praksa je približno 400 znakov---------------------------------

Ko je vsebina pripravljena, jo povlecite v podružnico v živo. Nato pojdite na [portal Alchemy partner](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje URL. 