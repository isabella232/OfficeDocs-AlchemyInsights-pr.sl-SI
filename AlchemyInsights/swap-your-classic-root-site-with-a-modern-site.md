---
title: Zamenjava klasičnega korenskega mesta s sodobnim mestom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691195"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="561fd-102">Zamenjava klasičnega korenskega mesta s sodobnim mestom</span><span class="sxs-lookup"><span data-stu-id="561fd-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="561fd-103">Če je bilo vaše okolje nastavljeno pred aprilom 2019, lahko korensko mesto spremenite na sodobno mesto tako, da uporabite Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="561fd-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="561fd-104">Če imate drugo mesto, ki ga želite uporabiti kot korensko mesto, ga lahko zamenjate [(zamenjate) s korenskim mestom](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="561fd-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="561fd-105">Uporabite funkcijo» [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) «, da zamenjate mesto mesta z drugim mestom, medtem ko arhivirate izvirno mesto.</span><span class="sxs-lookup"><span data-stu-id="561fd-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="561fd-106">Na voljo za spletno mesto skupine (ni povezano s skupino) in mesto za komunikacijo.</span><span class="sxs-lookup"><span data-stu-id="561fd-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="561fd-107">Dodatne zmogljivosti bodo kmalu predstavljene, tako da boste lahko uporabljali vsebino na spletnem mestu, vendar pretvorite obstoječe mesto na spletno mesto za komunikacijo.</span><span class="sxs-lookup"><span data-stu-id="561fd-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="561fd-108">Te zmogljivosti bodo postopoma razoblikovane.</span><span class="sxs-lookup"><span data-stu-id="561fd-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="561fd-109">Nadaljujte s preverjanjem središča za sporočila za posodobitve.</span><span class="sxs-lookup"><span data-stu-id="561fd-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="561fd-110">Znane težave s spletnimi mesti za zamenjavo</span><span class="sxs-lookup"><span data-stu-id="561fd-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="561fd-111">Ciljno mesto lahko vrne napako» not found «(HTTP 404) za kratek čas.</span><span class="sxs-lookup"><span data-stu-id="561fd-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="561fd-112">Vsebino bo treba znova preiskati in posodobiti indeks iskanja.</span><span class="sxs-lookup"><span data-stu-id="561fd-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="561fd-113">Ni potrebnega ročnega koraka – to bo samodejno opravljeno.</span><span class="sxs-lookup"><span data-stu-id="561fd-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="561fd-114">Vse, kar je odvisno od povezav» statičnih «(na primer sinhronizacije datotek in datotek programa OneNote), bo treba ročno popraviti.</span><span class="sxs-lookup"><span data-stu-id="561fd-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="561fd-115">Če je bilo izvorno mesto mesto organizacije novic, posodobite spletni naslov.</span><span class="sxs-lookup"><span data-stu-id="561fd-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="561fd-116">Pridobite seznam vseh lokacij z novicami organizacije.</span><span class="sxs-lookup"><span data-stu-id="561fd-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="561fd-117">Če želite zagotoviti, da so še vedno pravilno povezani, je treba potrditi mesta strežnika Project Server.</span><span class="sxs-lookup"><span data-stu-id="561fd-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
