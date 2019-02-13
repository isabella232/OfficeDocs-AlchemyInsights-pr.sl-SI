---
title: Omejevanje dostopa v SharePoint ali OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905164"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Omejevanje dostopa v SharePoint ali OneDrive

V SharePoint in OneDrive, omejite dostop do predmetov, kot so datoteke, mape in sezname z odobritvijo dostopa le za skupine ali posamezniki, ki želite imeti dostop. Privzeto dovoljenja v SharePoint dedujejo iz višje v hierarhiji. Tako datoteko podeduje njena dovoljenja v mapi, ki podeduje njeno dovoljenja iz knjižnice, ki je njena dovoljenja podedovana.
  
Delite na višji ravni (kot z delitvijo celotno spletno mesto) in nato prekiniti dedovanje, če ne želite, da delijo vse elemente na spletni strani. Vendar, ne priporočamo to saj omogoča ohranitev dovoljenja bolj kompleksnih in zavajajoče v prihodnosti. Tukaj je, kaj bi vam namesto tega:
  
- Če na primer želite deliti vsebino mape, razen za eno datoteko, premakniti to datoteko na novo lokacijo, ki ni v skupni rabi.
    
- Če imate dva podmape v mapi, in želite deliti eno podmapo z skupin A in B in dovoljujejo le skupina A drugi podmapo, delež nadrejeno mapo s skupino A in skupine B dodati prvo podmapo.
    
[Ustavi skupno rabo datoteko ali mapo](https://go.microsoft.com/fwlink/?linkid=2008861)
  

