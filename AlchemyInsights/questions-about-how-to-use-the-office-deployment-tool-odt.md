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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="e6d43-102">Vprašanja o uporabi orodja za uvajanje sistema Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="e6d43-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="e6d43-103">Prenesite orodje za uvajanje sistema Office iz [Microsoftovega središča za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="e6d43-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="e6d43-104">Ko prenesete datoteko, zaženite samoekstrahiranje izvršljive datoteke, ki vsebuje orodje za uvajanje sistema Office (setup.exe) in datoteko s konfiguracijo vzorca (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="e6d43-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="e6d43-105">**Če želite izključiti ali odstraniti aplikacije Microsoft 365 za izdelke podjetja iz odjemalskih računalnikov:**</span><span class="sxs-lookup"><span data-stu-id="e6d43-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="e6d43-106">Pri nameščanju programov Microsoft 365 za podjetja lahko izključite določene izdelke.</span><span class="sxs-lookup"><span data-stu-id="e6d43-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="e6d43-107">To naredite tako, da upoštevate navodila za namestitev Officea z datoteko ODT, vendar vključite element ExcludeApp v konfiguracijski datoteki.</span><span class="sxs-lookup"><span data-stu-id="e6d43-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="e6d43-108">Ta konfiguracijska datoteka na primer namesti vse aplikacije Microsoft 365 za izdelke Enterprise, razen Publisherja:</span><span class="sxs-lookup"><span data-stu-id="e6d43-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="e6d43-109">Pregled orodja za uvedbo sistema Office</span><span class="sxs-lookup"><span data-stu-id="e6d43-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

