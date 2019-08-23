---
title: Vprašanja o tem, kako uporabljati orodje za uvajanje Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36553556"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vprašanja o tem, kako uporabljati orodje za uvajanje Office (ODT)

Urad razvitje orodje prenesete iz [Microsoftovega centra za prenose](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po prenosu datoteke, zaženite samo pridobivanja izvedljivo datoteko, ki vsebuje Office razvitje orodje izvršljiv (setup.exe) in vzorec konfiguracijske datoteke (configuration.xml).
  
 **Izključiti ali odstraniti Office 365 ProPlus izdelkov iz odjemalske računalnike:**
  
Ko namestite Office 365 ProPlus, izključite lahko določene izdelke. To storite tako, sledite korakom za namestitev Office z na ODT, vendar vsebuje ExcludeApp elementa v konfiguracijski datoteki. Na primer, te konfiguracijske datoteke namesti vse Office 365 ProPlus proizvodov razen založnik:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled orodja za uvajanje urad](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

