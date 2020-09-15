---
title: Odpiranje z raziskovalcem ne deluje
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694472"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="2f2dd-102">Odpiranje z raziskovalcem ne deluje</span><span class="sxs-lookup"><span data-stu-id="2f2dd-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="2f2dd-103">Če je možnost» **Odpri z raziskovalcem** «ali» **pogled «v Raziskovalcu** ne **deluje, se** prepričajte, da je storitev za odjemalca nastavljena tako, da upošteva spodnja navodila.</span><span class="sxs-lookup"><span data-stu-id="2f2dd-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="2f2dd-104">Če se storitev ne izvaja, lahko na primer traja dolgo časa, da odprete SharePointovo ali OneDrive knjižnico.</span><span class="sxs-lookup"><span data-stu-id="2f2dd-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="2f2dd-105">V iskalno polje sistema Windows vnesite Run (Zaženi namizni program), vnesite Services. msc in nato izberite **Enter**.</span><span class="sxs-lookup"><span data-stu-id="2f2dd-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="2f2dd-106">Pomaknite se navzdol do storitve za odjemalca in preverite stolpec **stanje** .</span><span class="sxs-lookup"><span data-stu-id="2f2dd-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="2f2dd-107">Če se stanje storitve za samopostrežne stranke ne **izvaja**, dvokliknite storitev, kliknite **Start**in nato še **v redu**.</span><span class="sxs-lookup"><span data-stu-id="2f2dd-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2f2dd-108">Če je potrebno, omogočite storitev tako, da izberete **ročno** ali **samodejno** v polju **Vrsta zagona** .</span><span class="sxs-lookup"><span data-stu-id="2f2dd-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2f2dd-109">Če želite odpraviti težave z odpiranjem v Raziskovalcu, glejte [odpiranje v Raziskovalcu](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="2f2dd-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2f2dd-110">Raziščite sinhronizacijo kot boljšo alternativo: [sinhronizacija SharePointovih datotek z novim odjemalcem sinhronizacije za OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="2f2dd-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

