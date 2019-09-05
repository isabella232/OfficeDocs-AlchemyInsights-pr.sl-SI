---
title: Odpravljanje težav z uporabo odprte z raziskovalcem
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742749"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="93c50-102">Odpravljanje težav z odprtimi z raziskovalcem</span><span class="sxs-lookup"><span data-stu-id="93c50-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="93c50-103">Odpravljanje pogostih težav pri odpiranju knjižnice dokumentov v SharePointu ali storitvi OneDrive z ukazom» **Odpri z raziskovalcem** «:</span><span class="sxs-lookup"><span data-stu-id="93c50-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="93c50-104">Uporabite Internet Explorer 10 ali Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="93c50-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="93c50-105">**Plan s raziskovalec** isnt ' združljiv s mikroskop rob, varljiva žoga rumena barva, kresnica ter drugi.</span><span class="sxs-lookup"><span data-stu-id="93c50-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="93c50-106">**Plan s raziskovalec** je nesposoben v vsi browsers razen stažist v bolnišnici raziskovalec.</span><span class="sxs-lookup"><span data-stu-id="93c50-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="93c50-107">**Odprto z raziskovalcem** ni na voljo v sodobni izkušnji za SharePointove knjižnice.</span><span class="sxs-lookup"><span data-stu-id="93c50-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="93c50-108">Namesto tega uporabite **pogled v Raziskovalcu** .</span><span class="sxs-lookup"><span data-stu-id="93c50-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="93c50-109">**V Raziskovalcu izberite pogled** **možnosti** \> pogleda.</span><span class="sxs-lookup"><span data-stu-id="93c50-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="93c50-110">Pogled v Raziskovalcu ni združljiv z Microsoft Edge, Google Chrome, Firefox in drugi.</span><span class="sxs-lookup"><span data-stu-id="93c50-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="93c50-111">**Pogled v Raziskovalcu** , ki je na voljo samo v Internet Explorerju.</span><span class="sxs-lookup"><span data-stu-id="93c50-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="93c50-112">Preverite, ali se storitev WebClient izvaja.</span><span class="sxs-lookup"><span data-stu-id="93c50-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="93c50-113">V iskalno polje Windows vnesite Zaženi, izberite Zaženi namizno aplikacijo, vnesite Services. msc in pritisnite ENTER.</span><span class="sxs-lookup"><span data-stu-id="93c50-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="93c50-114">Pomaknite se navzdol do storitve WebClient in se prepričajte, da je v stolpcu **stanje** prikazano» tek «.</span><span class="sxs-lookup"><span data-stu-id="93c50-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="93c50-115">Če ne, dvokliknite storitev, kliknite **Start**in nato **v redu**.</span><span class="sxs-lookup"><span data-stu-id="93c50-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="93c50-116">(Morda boste morali najprej omogočiti storitev tako, da v polju **Vrsta zagona** izberete bodisi **ročno** bodisi **samodejno** .)</span><span class="sxs-lookup"><span data-stu-id="93c50-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="93c50-117">Odpiranje knjižnice v raziskovalcu je priročno, če morate enkrat kopirati ali premikati več datotek in map, če pa želite redno delati v knjižnici, priporočamo, da jo sinhronizirate.</span><span class="sxs-lookup"><span data-stu-id="93c50-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="93c50-118">Če želite odpraviti težave pri odpiranju v Raziskovalcu, glejte [Odpri v Raziskovalcu](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="93c50-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="93c50-119">Če želite več informacij o nastavitvi sinhronizacije, glejte [sinhronizacija SharePointovih datotek z novim odjemalcem za sinhronizacijo storitve OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="93c50-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="93c50-120">Prosimo, glejte članek [Kako uporabljati ukaz» Odpri z raziskovalcem «, da odpravite težave v SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) za več informacij.</span><span class="sxs-lookup"><span data-stu-id="93c50-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

