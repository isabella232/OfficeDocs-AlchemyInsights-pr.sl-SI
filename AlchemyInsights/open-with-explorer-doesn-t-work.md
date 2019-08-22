---
title: Odpri z Explorer ne deluje
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538503"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="96c9e-102">Odpri z Explorer ne deluje</span><span class="sxs-lookup"><span data-stu-id="96c9e-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="96c9e-103">Če **Odpri v Raziskovalcu** ali **pogled v Raziskovalcu datoteke** ne deluje, se prepričajte, WebClient storitev, ki **teče** po spodnjih navodilih.</span><span class="sxs-lookup"><span data-stu-id="96c9e-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="96c9e-104">Na primer, bo trajalo dolgo časa, da odprete knjižnico SharePoint ali OneDrive, ko se storitev ne izvaja.</span><span class="sxs-lookup"><span data-stu-id="96c9e-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="96c9e-105">V okno polje za iskanje, vrsta teči, izberite prost dostop pult app, vnesite services.msc in izberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="96c9e-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="96c9e-106">Pomaknite se do WebClient storitev in preverite stolpec **stanje** .</span><span class="sxs-lookup"><span data-stu-id="96c9e-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="96c9e-107">Če WebClient storitve stanja ni **tekmovanje v teku**, dvokliknite storitve, kliknite **Start**in nato kliknite v **redu**.</span><span class="sxs-lookup"><span data-stu-id="96c9e-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="96c9e-108">Omogočiti storitev, če je potrebno, tako, da izberete **ročno** ali **avtomatsko** v polje **Vrsta zagona** .</span><span class="sxs-lookup"><span data-stu-id="96c9e-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="96c9e-109">Odpravljanje težav v datoteko Explorer, glejte [plan v raziskovalec](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="96c9e-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="96c9e-110">Raziskati sinhronizacijo kot boljša alternativa: [sinhronizacijo SharePointovih datotek z novo OneDrive sinhronizacijo odjemalca](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="96c9e-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

