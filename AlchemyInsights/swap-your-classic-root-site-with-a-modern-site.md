---
title: Zamenjajte svojo klasično korensko stran s sodobno spletno stran
ms.author: pebaum
author: pebaum
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: fe1f0f662c49de2bd0b5b997697c98309cb7983f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042943"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="a4948-102">Zamenjajte svojo klasično korensko stran s sodobno spletno stran</span><span class="sxs-lookup"><span data-stu-id="a4948-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="a4948-103">Če je bilo vaše okolje nastavljeno pred aprilom 2019, lahko korensko mesto spremenite na moderno spletno mesto z uporabo Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="a4948-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="a4948-104">Če imate drugačno spletno mesto, ki ga želite uporabiti kot korensko mesto, lahko z njim zamenjate [(swap) korensko mesto](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="a4948-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="a4948-105">Uporaba [sklicevati-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamenjati lokacijo mesta z drugo spletno stran, medtem ko arhiviranje izvirno mesto.</span><span class="sxs-lookup"><span data-stu-id="a4948-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="a4948-106">Na voljo za obe strani skupine (ni povezan s skupino) in mesto za komunikacijo.</span><span class="sxs-lookup"><span data-stu-id="a4948-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="a4948-107">Dodatne zmogljivosti bodo uvedene kmalu, da vam bo omogočilo, da uporabljajo vsebino na spletni strani, vendar pretvoriti obstoječe mesto na komunikacijsko mesto.</span><span class="sxs-lookup"><span data-stu-id="a4948-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="a4948-108">Te zmogljivosti bodo postopoma izpeljali.</span><span class="sxs-lookup"><span data-stu-id="a4948-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="a4948-109">Še naprej preverite Office 365 Message center za posodobitve.</span><span class="sxs-lookup"><span data-stu-id="a4948-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="a4948-110">Znane težave s zamenjavo strani</span><span class="sxs-lookup"><span data-stu-id="a4948-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="a4948-111">Ciljna stran lahko za kratek čas vrne napako» ni mogoče najti «(HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="a4948-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="a4948-112">Vsebino bo treba ponovno prejeti, da posodobite indeks iskanja.</span><span class="sxs-lookup"><span data-stu-id="a4948-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="a4948-113">Ni potreben ročni korak-to se bo zgodilo samodejno.</span><span class="sxs-lookup"><span data-stu-id="a4948-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="a4948-114">Vse odvisno od "statičnih" povezav (kot so file Sync in OneNote datoteke) bo treba ročno popraviti.</span><span class="sxs-lookup"><span data-stu-id="a4948-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="a4948-115">Če je izvorna stran organizacijska stran z novicami, posodobite URL.</span><span class="sxs-lookup"><span data-stu-id="a4948-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="a4948-116">Pridobite seznam vseh strani z organizacijskimi novicami.</span><span class="sxs-lookup"><span data-stu-id="a4948-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="a4948-117">Mesta strežnika Project Server je morda treba potrditi, da se zagotovi, da so še vedno pravilno povezani.</span><span class="sxs-lookup"><span data-stu-id="a4948-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





