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
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419888"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="e9169-102">Odpri z Explorer ne deluje</span><span class="sxs-lookup"><span data-stu-id="e9169-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="e9169-103">Če **Odpri v Raziskovalcu** ali **pogled v Raziskovalcu datoteke** ne deluje, se prepričajte, WebClient storitev, ki **teče** po spodnjih navodilih.</span><span class="sxs-lookup"><span data-stu-id="e9169-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="e9169-104">Na primer, bo trajalo dolgo časa, da odprete knjižnico SharePoint ali OneDrive, ko se storitev ne izvaja.</span><span class="sxs-lookup"><span data-stu-id="e9169-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="e9169-105">V okno polje za iskanje, vrsta teči, izberite prost dostop pult app, vnesite services.msc in izberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="e9169-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="e9169-106">Pomaknite se do WebClient storitev in preverite stolpec **stanje** .</span><span class="sxs-lookup"><span data-stu-id="e9169-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="e9169-107">Če WebClient storitve stanja ni **tekmovanje v teku**, dvokliknite storitve, kliknite **Start**in nato kliknite v **redu**.</span><span class="sxs-lookup"><span data-stu-id="e9169-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e9169-108">Omogočiti storitev, če je potrebno, tako, da izberete **ročno** ali **avtomatsko** v polje **Vrsta zagona** .</span><span class="sxs-lookup"><span data-stu-id="e9169-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e9169-109">Odpravljanje težav v datoteko Explorer, glejte [plan v raziskovalec](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="e9169-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e9169-110">Raziskati sinhronizacijo kot boljša alternativa: [sinhronizacijo SharePointovih datotek z novo OneDrive sinhronizacijo odjemalca](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e9169-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

