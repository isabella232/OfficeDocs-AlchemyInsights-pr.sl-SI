---
title: Nadzorovanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702919"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Nadzorovanje pogojnega dostopa za Exchange

Uporabniki, ki so usmerjeni s pogojnim dostopom, bodo prejeli e-poštno obvestilo, če ne ustrezajo zahtevam za dostop do vaše organizacije. Če želite razrešiti, priporočamo eno ali več od teh rešitev:
  
- Če je naprava domnevno včlanjena, svetuje uporabniku, da se poišče v programu podjetja portal in preveri, ali je prikazana v portalu podjetja. Če ne, mora uporabnik vpisati napravo.
    
- V portalu Azure se pozanimajte o ** \> skladnosti naprave**. V razdelku **monitor** kliknite **skladnost naprave**. Če želite preveriti, ali je naprava uporabnika označena kot združljiva, si oglejte poročilo o skladnosti naprave. 
    
- V portalu Azure se pozanimajte o ** \> skladnosti naprave**. V razdelku **upravljanje**kliknite **Pravilniki**. Na seznamu pravilnikov o skladnosti preverite, ali je profil dodeljen napravi uporabnika. Če ni dodeljen noben profil, InTune ne more potrditi stanja skladnosti naprave. 
    
- Uredite uporabnikovo pogojno dostopno dodelitev.
    
1. V portalu Azure se pozanimajte za **InTune \> \> pravilnika za pogojni dostop**
    
2. Izbira pravilnika s seznama
    
3. Kliknite **Uporabniki in skupine**
    
4. Če želite določene pravilnike usmeriti na osebo, jih dodajte na seznam **vključi** . Če želite zagotoviti, da je oseba izpuščena iz pravilnika, jih dodajte na seznam **izključi** . 
    
Preberite več [o tem: Kako spremljati naprave s pogojnim dostopom](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

