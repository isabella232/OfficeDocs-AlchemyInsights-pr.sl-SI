---
title: Uporaba brskalnika Microsoft Edge, ki temelji na brskalnikih Chromium za izvoz E-odkrivanja
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834387"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="21783-102">Uporaba brskalnika Microsoft Edge, ki temelji na brskalnikih Chromium za izvoz E-odkrivanja</span><span class="sxs-lookup"><span data-stu-id="21783-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="21783-103">Zaradi nedavne spremembe brskalniki Microsoft Edge ne bodo več privzeto omogočili podpore za ClickOnce.</span><span class="sxs-lookup"><span data-stu-id="21783-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="21783-104">Če želite še naprej uporabljati orodje za izvoz e-odkrivanja v storitvi Microsoft 365, morate bodisi uporabiti Microsoft Internet Explorer ali omogočiti podporo za ClickOnce v brskalniku Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="21783-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="21783-105">Če želite omogočiti podporo za ClickOnce v brskalniku Microsoft Edge na osnovi brskalnika Chromium:</span><span class="sxs-lookup"><span data-stu-id="21783-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="21783-106">V brskalniku Microsoft Edge obiščite spletno edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="21783-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="21783-107">Za možnost Podpora za ClickOnce  spremenite vrednost iz Privzeto ali **Onemogočeno** **v Omogočeno.**</span><span class="sxs-lookup"><span data-stu-id="21783-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="21783-108">Na dnu okna brskalnika izberite Znova **zaženi**.</span><span class="sxs-lookup"><span data-stu-id="21783-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="21783-109">Sprememba bo veljati po vnovičnem zagonu brskalnika Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="21783-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="21783-110">Če želite več informacij o tem in korakih za namestitev orodja za izvoz, glejte: [Izvoz rezultatov iskanja vsebine.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="21783-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>