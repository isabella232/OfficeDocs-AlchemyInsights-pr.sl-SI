---
title: Sodobna stran kot korensko mesto
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753920"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="45f4b-102">Sodobna stran kot root stran</span><span class="sxs-lookup"><span data-stu-id="45f4b-102">Modern site as root site</span></span>

<span data-ttu-id="45f4b-103">Začeli smo, da uvajanje nove funkcije, ki vam bo omogočilo, da [swap vaše klasično stran root stran s sodobno spletno stran](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="45f4b-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="45f4b-104">Uporaba [sklicevati-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) zamenjati lokacijo mesta z drugo spletno stran, medtem ko arhiviranje izvirno mesto.</span><span class="sxs-lookup"><span data-stu-id="45f4b-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="45f4b-105">Na voljo za obe strani skupine (ni povezan s skupino) in mesto za komunikacijo.</span><span class="sxs-lookup"><span data-stu-id="45f4b-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="45f4b-106">Ne izbrišite klasične korenske strani, da ustvarite sodobno komunikacijsko mesto.</span><span class="sxs-lookup"><span data-stu-id="45f4b-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="45f4b-107">Microsoft tega ne podpira.</span><span class="sxs-lookup"><span data-stu-id="45f4b-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="45f4b-108">Če izbrišete korensko mesto, bodo vsa SharePointova mesta v vaši organizaciji nedostopna vsem uporabnikom, dokler ne obnovite mesta ali ustvarite novega mesta na istem URL-ju.</span><span class="sxs-lookup"><span data-stu-id="45f4b-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="45f4b-109">To funkcijo bomo komunicirali prek centra za sporočila.</span><span class="sxs-lookup"><span data-stu-id="45f4b-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="45f4b-110">Pričakovati je, da bo funkcija v kratkem vklopljena v najemniku.</span><span class="sxs-lookup"><span data-stu-id="45f4b-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="45f4b-111">Znane težave s zamenjavo strani</span><span class="sxs-lookup"><span data-stu-id="45f4b-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="45f4b-112">Ciljna stran lahko za kratek čas vrne napako» ni mogoče najti «(HTTP 404).</span><span class="sxs-lookup"><span data-stu-id="45f4b-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="45f4b-113">Vsebino bo treba ponovno prejeti, da posodobite indeks iskanja.</span><span class="sxs-lookup"><span data-stu-id="45f4b-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="45f4b-114">Tu ni ročnega koraka, ki je zahtevan tukaj, to se bo samodejno zgodilo.</span><span class="sxs-lookup"><span data-stu-id="45f4b-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="45f4b-115">Vse odvisno od "statičnih" povezav (kot so file Sync in OneNote datoteke) bo treba ročno popraviti.</span><span class="sxs-lookup"><span data-stu-id="45f4b-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="45f4b-116">Mesta strežnika Project Server je morda treba potrditi, da se zagotovi, da so še vedno pravilno povezani.</span><span class="sxs-lookup"><span data-stu-id="45f4b-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
