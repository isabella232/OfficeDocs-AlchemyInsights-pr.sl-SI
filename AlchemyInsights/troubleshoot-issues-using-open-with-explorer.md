---
title: Odpravljanje težav z odprto Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390623"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="c55d1-102">Odpravljanje težav z odprto s raziskovalec</span><span class="sxs-lookup"><span data-stu-id="c55d1-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="c55d1-103">Odpravite pogoste težave z odprtjem knjižnice dokumentov SharePoint ali OneDrive, uporabite ukaz **Odpri v Raziskovalcu** :</span><span class="sxs-lookup"><span data-stu-id="c55d1-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="c55d1-104">Z Internet Explorerjem 10 ali Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="c55d1-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="c55d1-105">**Odpri v Raziskovalcu** ni združljiv z Microsoft Edge, Google Chrome, Firefox in drugi.</span><span class="sxs-lookup"><span data-stu-id="c55d1-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c55d1-106">**Odpri v Raziskovalcu** onemogočena v vseh brskalnikih razen Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c55d1-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="c55d1-107">**Odpri v Raziskovalcu** ni na voljo v moderno izkušnjo za SharePointove knjižnice.</span><span class="sxs-lookup"><span data-stu-id="c55d1-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="c55d1-108">Namesto tega uporabite **pogled v Raziskovalcu datoteke** .</span><span class="sxs-lookup"><span data-stu-id="c55d1-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="c55d1-109">Izberite **možnosti pogleda** \> **pogled v Raziskovalcu datoteke**.</span><span class="sxs-lookup"><span data-stu-id="c55d1-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="c55d1-110">Pogled v Raziskovalcu datoteke ni združljiva z Microsoft Edge, Google Chrome, Firefox in drugi.</span><span class="sxs-lookup"><span data-stu-id="c55d1-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c55d1-111">**Pogled v Raziskovalcu datoteke** na voljo le v Internet Explorerju.</span><span class="sxs-lookup"><span data-stu-id="c55d1-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="c55d1-112">Preverite, ali je zagnana storitev, od WebClient.</span><span class="sxs-lookup"><span data-stu-id="c55d1-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="c55d1-113">V Windows iskalno polje, vnesite Zaženi, izberite prost dostop pult app, vnesite services.msc in pritisnite Enter.</span><span class="sxs-lookup"><span data-stu-id="c55d1-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="c55d1-114">Se pomaknite navzdol do WebClient storitev in se prepričajte v stolpcu **stanje** prikaže "Teče".</span><span class="sxs-lookup"><span data-stu-id="c55d1-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="c55d1-115">Če ne, dvokliknite storitve, kliknite **Start**in nato kliknite v **redu**.</span><span class="sxs-lookup"><span data-stu-id="c55d1-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c55d1-116">(Morda boste morali najprej omogočiti storitev tako, da izberete **ročno** ali **avtomatsko** v polje **Vrsta zagona** .)</span><span class="sxs-lookup"><span data-stu-id="c55d1-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c55d1-117">Otvoritev knjižnice v datoteko Explorer je priročno, če želite kopirati ali premakniti več datotek in map, ko, vendar če želite redno delo v knjižnici, priporočamo, da sinhronizirate.</span><span class="sxs-lookup"><span data-stu-id="c55d1-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="c55d1-118">Odpravljanje težav v datoteko Explorer, glejte [plan v raziskovalec](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="c55d1-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c55d1-119">Informacij o nastavitev sinhronizacije, glejte [Sinhroniziranje SharePointovih datotek z novo OneDrive sinhronizacijo odjemalca](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c55d1-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="c55d1-120">Prosimo, glejte članek [kako uporabite ukaz »Odpri z Explorer« težave v SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="c55d1-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

