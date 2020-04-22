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
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="ccbad-102">Odpri z raziskovalcem ne deluje</span><span class="sxs-lookup"><span data-stu-id="ccbad-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="ccbad-103">Če je **odprto z raziskovalcem** ali **pogledom v datoteki raziskovalec** ne deluje, poskrbite, da bo storitev WebClient nastavljena na **izvajanje** tako, da sledite spodnjim korakom.</span><span class="sxs-lookup"><span data-stu-id="ccbad-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="ccbad-104">Morda bo na primer dolgo trajalo, da odprete knjižnico SharePoint ali OneDrive, ko se storitev ne izvaja.</span><span class="sxs-lookup"><span data-stu-id="ccbad-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="ccbad-105">V iskalno polje Windows vnesite Zaženi, izberite Zaženi namizno aplikacijo, vnesite Services. msc in izberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="ccbad-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="ccbad-106">Pomaknite se navzdol do storitve WebClient in preverite stolpec **stanja** .</span><span class="sxs-lookup"><span data-stu-id="ccbad-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="ccbad-107">Če se stanje storitve WebClient ne **izvaja**, dvokliknite storitev, kliknite **Start**in nato **v redu**.</span><span class="sxs-lookup"><span data-stu-id="ccbad-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="ccbad-108">Če je potrebno, omogočite storitev tako, da v polju **Vrsta zagona** izberete **ročno** ali **samodejno** .</span><span class="sxs-lookup"><span data-stu-id="ccbad-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="ccbad-109">Če želite odpraviti težave pri odpiranju v Raziskovalcu, glejte [Odpri v Raziskovalcu](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="ccbad-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="ccbad-110">Raziščite sinhronizacijo kot boljšo alternativo: [sinhronizacija SharePointovih datotek z novim odjemalcem sinhronizacije storitve OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="ccbad-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

