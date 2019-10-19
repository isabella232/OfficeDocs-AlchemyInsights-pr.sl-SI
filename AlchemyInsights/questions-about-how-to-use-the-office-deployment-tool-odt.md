---
title: Vprašanja o uporabi orodja za uvajanje Officea (ODT)
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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553556"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="9e634-102">Vprašanja o uporabi orodja za uvajanje Officea (ODT)</span><span class="sxs-lookup"><span data-stu-id="9e634-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="9e634-103">Prenesite orodje za uvajanje Officea iz [Microsoftovega centra za prenose](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="9e634-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="9e634-104">Čez downloading pila, prost dostop svoja osebnost-izvor izvršljiv pila, kateri vsebovati urad razvitje orodje izvršljiv (setup. exe) ter a vzorec zunanja podoba pila (Configuration. xml).</span><span class="sxs-lookup"><span data-stu-id="9e634-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="9e634-105">**Če želite izključiti ali odstraniti izdelke sistema Office 365 ProPlus iz odjemalskih računalnikov:**</span><span class="sxs-lookup"><span data-stu-id="9e634-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="9e634-106">Pri nameščanju Officea 365 ProPlus lahko izključite določene izdelke.</span><span class="sxs-lookup"><span data-stu-id="9e634-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="9e634-107">To storite tako, da sledite navodilom za namestitev Officea z ODT, vendar vključite element ExcludeApp v konfiguracijsko datoteko.</span><span class="sxs-lookup"><span data-stu-id="9e634-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="9e634-108">Ta konfiguracijska datoteka na primer namesti vse izdelke sistema Office 365 ProPlus, razen Publisherja:</span><span class="sxs-lookup"><span data-stu-id="9e634-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="9e634-109">Pregled orodja za uvajanje Officea</span><span class="sxs-lookup"><span data-stu-id="9e634-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

