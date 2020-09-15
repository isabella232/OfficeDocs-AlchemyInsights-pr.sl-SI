---
title: Odpravljanje težav z odpiranjem z raziskovalcem
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659074"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="fb1f1-102">Odpravljanje težav z odpiranjem z raziskovalcem</span><span class="sxs-lookup"><span data-stu-id="fb1f1-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="fb1f1-103">Odpravljanje pogostih težav z odpiranjem knjižnice dokumentov v SharePointu ali OneDrive z ukazom» **Odpri z raziskovalcem** «:</span><span class="sxs-lookup"><span data-stu-id="fb1f1-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="fb1f1-104">Uporabite Internet Explorer 10 ali Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="fb1f1-105">**Odpiranje z raziskovalcem** ni združljivo z brskalnikom Microsoft Edge, Google Chrome, Firefox in drugimi.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="fb1f1-106">**Odpiranje z raziskovalcem** je onemogočeno v vseh brskalnikih, razen v Internet Explorerju.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="fb1f1-107">**Odpiranje z raziskovalcem** ni na voljo v sodobni izkušnji za SharePointove knjižnice.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="fb1f1-108">Namesto tega uporabite **pogled v Raziskovalcu** .</span><span class="sxs-lookup"><span data-stu-id="fb1f1-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="fb1f1-109">V Raziskovalcu izberite pogled **možnosti pogleda** \> **View in File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="fb1f1-110">Pogled v Raziskovalcu ni združljiv s programom Microsoft Edge, Google Chrome, Firefox in drugimi.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="fb1f1-111">**Pogled v Raziskovalcu** , ki je na voljo le v Internet Explorerju.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="fb1f1-112">Prepričajte se, da je storitev za odjemalca zagnana.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="fb1f1-113">V iskalno polje sistema Windows vnesite Run (Zaženi namizni program), vnesite Services. msc in nato pritisnite tipko ENTER.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="fb1f1-114">Pomaknite se navzdol do storitve za odjemalca in se prepričajte, da je v stolpcu **stanje** prikazano» zagnano «.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="fb1f1-115">Če ni, dvokliknite storitev, kliknite **Start**in nato **v redu**.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="fb1f1-116">(Morda boste morali najprej omogočiti storitev tako, da izberete **ročno** ali **samodejno** v polju **Vrsta zagona** .)</span><span class="sxs-lookup"><span data-stu-id="fb1f1-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="fb1f1-117">Odpiranje knjižnice v raziskovalcu je priročno, če morate enkrat kopirati ali premakniti več datotek in map, če pa želite redno delati v knjižnici, priporočamo, da jo sinhronizirate.</span><span class="sxs-lookup"><span data-stu-id="fb1f1-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="fb1f1-118">Če želite odpraviti težave z odpiranjem v Raziskovalcu, glejte [odpiranje v Raziskovalcu](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="fb1f1-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="fb1f1-119">Če želite več informacij o nastavitvi sinhronizacije, glejte [sinhronizacija SharePointovih datotek z novim odjemalcem sinhronizacije za OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="fb1f1-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="fb1f1-120">Če želite več informacij, preberite članek [Uporaba ukaza» Odpri z raziskovalcem «za odpravljanje težav v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="fb1f1-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

