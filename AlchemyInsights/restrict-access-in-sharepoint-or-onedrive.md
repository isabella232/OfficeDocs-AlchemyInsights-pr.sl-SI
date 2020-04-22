---
title: Omejevanje dostopa v SharePointu ali storitvi OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715900"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omejevanje dostopa v SharePointu ali storitvi OneDrive

V SharePointu in storitvi OneDrive omejite dostop do elementov, kot so datoteke, mape in seznami, tako da omogočite dostop samo skupinam ali posameznikom, ki jih želite imeti dostop. Dovoljenja v SharePointu so privzeto podedovana od višje v hierarhiji. Torej datoteka dedi dovoljenja iz mape, ki dedi dovoljenja iz knjižnice, ki dedi svoja dovoljenja iz mesta.
  
Lahko delite na višji ravni (na primer z delitvijo celotno mesto) in nato prekinil dedovanje, če ne želite deliti vse elemente na mestu. Vendar pa tega ne priporočamo, ker omogoča ohranitev dovoljenj bolj zapletena in nejasna v prihodnosti. Tukaj je, kaj lahko storite namesto tega:
  
- Če želite na primer deliti vso vsebino mape, razen ene datoteke v njej, premaknite to datoteko na novo mesto, ki ni v skupni rabi.
    
- Če imate v mapi dve podmapi in želite deliti eno podmapo s skupinami A in B in dovoliti samo skupini A dostop do druge podmape, delite nadrejeno mapo s skupino A in dodajte skupino B v prvo podmapo.
    
[Ustavitev skupne rabe datoteke ali mape](https://go.microsoft.com/fwlink/?linkid=2008861)
  

