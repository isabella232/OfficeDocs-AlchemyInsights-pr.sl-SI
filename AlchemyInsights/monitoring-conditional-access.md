---
title: Spremljanje pogojnega dostopa
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902378"
---
# <a name="monitoring-conditional-access"></a>Spremljanje pogojnega dostopa

Uporabniki, ki so usmerjena s pogojnim dostopom prejmejo oznanilo email, če izpolnjuje zahteve vaše organizacije. Odločiti, priporočamo, da eden ali več od naslednjih rešitev:
  
- Če naprava je domneva, da bodo vpisani, svetuje uporabnik iti podjetje Portal app in preveri, da se pojavi v portalu podjetja. Če ne, uporabnik vpisati naprave.
    
- V portalu Azure iti **Intune \> skladnost naprave**. Pod **oknom** kliknite **napravo skladnosti**. Poglej si poročilo skladnost naprave za preverjanje, da uporabnikova naprava je označena kot skladna. 
    
- V portalu Azure iti **Intune \> skladnost naprave**. Pod **upravljanje**, kliknite **pravila**. Na seznamu skladnost politik, preverite, ali da je dodeljen profil vaš uporabnik naprave. Če je dodeljena brez profila, Intune ne bo zmožen potrditi skladnost stanje naprave. 
    
- Urejanje dodelitev pogojnega dostopa uporabnika.
    
1. V portalu Azure iti **Intune \> pogojni dostop \> pravila**
    
2. Na seznamu izberite politike
    
3. Kliknite **Uporabniki in skupine**
    
4. Cilj politike na nekoga, jih dodajte na seznam **vključitev** . Če želite zagotoviti, da oseba izpustite iz pravilnika, dodati na seznam **izključitev** . 
    
Preberite več: [Kako Monitor pogojnem dostopu naprave](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

