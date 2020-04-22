---
title: Odpri z raziskovalcem ne deluje
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713050"
---
# <a name="open-with-explorer-isnt-working"></a>Odpri z raziskovalcem ne deluje

Če je **odprto z raziskovalcem** ali **pogledom v datoteki raziskovalec** ne deluje, poskrbite, da bo storitev WebClient nastavljena na **izvajanje** tako, da sledite spodnjim korakom. Morda bo na primer dolgo trajalo, da odprete knjižnico SharePoint ali OneDrive, ko se storitev ne izvaja. 
  
1. V iskalno polje Windows vnesite Zaženi, izberite Zaženi namizno aplikacijo, vnesite Services. msc in izberite **Enter**.
    
2. Pomaknite se navzdol do storitve WebClient in preverite stolpec **stanja** . Če se stanje storitve WebClient ne **izvaja**, dvokliknite storitev, kliknite **Start**in nato **v redu**. Če je potrebno, omogočite storitev tako, da v polju **Vrsta zagona** izberete **ročno** ali **samodejno** . 
    
> [!NOTE]
> Če želite odpraviti težave pri odpiranju v Raziskovalcu, glejte [Odpri v Raziskovalcu](https://go.microsoft.com/fwlink/?linkid=871665). Raziščite sinhronizacijo kot boljšo alternativo: [sinhronizacija SharePointovih datotek z novim odjemalcem sinhronizacije storitve OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

