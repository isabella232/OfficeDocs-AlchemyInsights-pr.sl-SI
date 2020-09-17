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
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774907"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vprašanja o uporabi orodja za uvajanje sistema Office (ODT)

Prenesite orodje za uvajanje sistema Office iz [Microsoftovega središča za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Ko prenesete datoteko, zaženite samoekstrahiranje izvršljive datoteke, ki vsebuje orodje za uvajanje sistema Office (setup.exe) in datoteko s konfiguracijo vzorca (configuration.xml).
  
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
  

