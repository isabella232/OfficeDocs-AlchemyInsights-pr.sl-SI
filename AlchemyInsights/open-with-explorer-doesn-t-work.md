---
title: »Odpri v Raziskovalcu« ne deluje
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011352"
---
# <a name="open-with-explorer-isnt-working"></a>Odpri v Raziskovalcu ne deluje

Če **»Odpri v Raziskovalcu«** **ali** »Prikaži v Raziskovalcu« ne deluje, preverite, ali je storitev WebClient nastavljena na **Se** izvaja tako, da sledite spodnjim korakom. Na primer, morda bo trajalo dolgo časa, da se odpre SharePoint ali OneDrive, če se storitev ne izvaja. 
  
1. V Windows polje vnesite zaženi, izberite namizno aplikacijo Zaženi, vnesite services.msc in nato izberite **Vnesi**.
    
2. Pomaknite se navzdol do storitve WebClient in preverite **stolpec Stanje.** Če se stanje storitve WebClient ne **izvaja,** dvokliknite storitev, kliknite **Zaženi** in nato V **redu.** Po potrebi omogočite storitev tako, da v **polju** Vrsta zagona **izberete** Ročno **ali** Samodejno. 
    
> [!NOTE]
> Če želite odpraviti težave z odpiranjem v Raziskovalcu, glejte [Odpiranje v Raziskovalcu.](https://go.microsoft.com/fwlink/?linkid=871665) Raziščite sinhronizacijo kot boljšo nadomestno rešitev: [sinhronizirajte SharePoint datotek z novim sinhronizacija s storitvijo OneDrive odjemalcem.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

