---
title: Vprašanja o uporabi orodja za uvedbo sistema Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790348"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vprašanja o uporabi orodja za uvedbo sistema Office (ODT)

Prenesite orodje za uvedbo sistema Office z Microsoftovega centra [za prenose.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Ko prenesete datoteko, zaženite samo ekstrahiranje izvedljive datoteke, ki vsebuje izvedljivo orodje za uvedbo sistema Office (setup.exe) in vzorčno konfiguracijsko datoteko (configuration.xml).
  
 **Če želite izključiti ali odstraniti Programe storitve Microsoft 365 za podjetja iz odjemalskih računalnikov:**
  
Ko nameščate programe storitve Microsoft 365 za podjetja, lahko izključite določene izdelke. Če želite to narediti, upoštevajte navodila za namestitev Officea z ODT, vendar vključite element ExcludeApp v konfiguracijsko datoteko. Ta konfiguracijska datoteka na primer namesti vse programe storitve Microsoft 365 za izdelke podjetja, razen Publisherja:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled orodja za uvedbo sistema Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

