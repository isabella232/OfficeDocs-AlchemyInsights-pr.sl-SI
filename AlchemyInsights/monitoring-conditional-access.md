---
title: Spremljanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713734"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Spremljanje pogojnega dostopa za Exchange

Uporabniki, usmerjeni s pogojnim dostopom, prejmejo e-poštno sporočilo z obvestilom, če ne izpolnjujejo zahtev za dostop vaše organizacije. Za rešitev priporočamo eno ali več naslednjih rešitev:
  
- Če se domneva, da je naprava vpisana v program, Svetujte uporabniku, da gre v aplikacijo portal podjetja, in preverite, ali je v portalu podjetja. Če se ne, mora uporabnik vpisati napravo.
    
- V portalu Azure pojdite na ** \> prilagajanje skladnosti naprave**. Pod **monitor** kliknite **skladnost naprave**. Oglejte si poročilo o skladnosti naprave, da preverite, ali je uporabniška naprava označena kot skladna. 
    
- V portalu Azure pojdite na ** \> prilagajanje skladnosti naprave**. V razdelku **upravljanje**kliknite **Pravilniki**. Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen uporabnikovi napravi. Če profil ni dodeljen, InTune ne bo mogel potrditi stanja skladnosti naprave. 
    
- Uredite uporabniški nalog za pogojni dostop.
    
1. V portalu Azure pojdite na **InTune \> pravilniki pogojnega \> dostopa**
    
2. Izbiranje pravilnika s seznama
    
3. Kliknite **Uporabniki in skupine**
    
4. Če želite na nekoga ciljati določeno politiko, jih dodajte na seznam **vključi** . Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jo dodajte na seznam **izključitev** . 
    
Preberite več: [kako nadzorovati naprave s pogojnim dostopom](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

