---
title: Vprašanja o uporabi orodja za uvajanje sistema Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086172"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vprašanja o uporabi orodja za uvajanje sistema Office (ODT)

Prenesite orodje za uvajanje sistema Office iz [Microsoftovega središča za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Ko prenesete datoteko, zaženite samoekstrahiranje izvršljive datoteke, ki vsebuje orodje za uvajanje sistema Office (setupodt.exe) in datoteko s konfiguracijo vzorca (configuration.xml).
  
 **Če želite izključiti ali odstraniti aplikacije Microsoft 365 za izdelke podjetja iz odjemalskih računalnikov:**
  
Pri nameščanju programov Microsoft 365 za podjetja lahko izključite določene izdelke. To naredite tako, da upoštevate navodila za namestitev Officea z datoteko ODT, vendar vključite element ExcludeApp v konfiguracijski datoteki. Ta konfiguracijska datoteka na primer namesti vse aplikacije Microsoft 365 za izdelke Enterprise, razen Publisherja:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled orodja za uvedbo sistema Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

