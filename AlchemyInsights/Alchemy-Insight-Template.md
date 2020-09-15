---
title: enako kot ime datoteke je najboljše
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
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664150"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Zahtevani Alchemy header H1, H2's ne delujejo."
Najboljše prakse in smernice za ustvarjanje avtorjev alkimije:

1. **Do not Nest vpogledov v mape**– to bo prekinilo strukturo URL-ja. Poskušamo popraviti to.
1. Datoteke v mapi **AlchemyInsights** morajo imeti male datoteke z vezaji za presledke ex. ***navodila za omogočanje uporabe v sporu – pridržite***.
    1. Vključite ID pravila ali ID vedra na [partnerskem portalu Alchemy](https://alchemyportal.azurewebsites.net) v polju MS. po meri. ex. ***MS. Custom: 100021***
1. Uporabite preostala metapodatka na vrhu te datoteke kot predlogo.
1. V [partnerskem portalu Alchemy](https://alchemyportal.azurewebsites.net)se pomaknite do razdelka» **naslov stranke vpogleda «:** in uporabite to kot izhodišče za vaš naslov H1 za vpogled. 
    > [!NOTE]
    > V programu Alchemy vpogledi morajo biti le en H1 na vrhu ali pa bodo vdrli v proizvodnjo. H2s ne omogoča uporabe **krepkih** ali drugih konvencij, da bi označili ločene odseke.
1. Nato vnesite besedilo v telo z uporabo osnutka gradiva v razdelku» vpogledi v stranke «na strani» pravilo Alchemy «
    1. Označeni seznami so Fini
    1. Tudi oštevilčeni seznami
    1. **Krepko** in *Ležeče* so a-ok
    1. Povezave bi morale biti vedno **» povezave do spleta «/External** ali **Deep povezave do elementov uporabniškega vmesnika**in ne notranjih povezav.
    1. Slike trenutno niso uradno podprte, vendar je to v načrtu.

In to je res že nekoliko predolgo. Najboljša praksa je približno 400 znakov---------------------------------

Ko je vaša vsebina pripravljena, jo potegnite v živo vejo. Nato pojdite na portal za [partnerje Alchemy](https://alchemyportal.azurewebsites.net) in vnesite ime datoteke v polje URL. 