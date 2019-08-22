---
title: Sodobno mesto kot korensko mesto
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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543869"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="29c3a-102">Sodobno mesto kot korensko mesto</span><span class="sxs-lookup"><span data-stu-id="29c3a-102">Modern site as root site</span></span>

<span data-ttu-id="29c3a-103">Smo začeli uvajanje novost, ki bo omogočilo, da zamenjate vaš vzoren mesto korensko mesto z moderno mesto.</span><span class="sxs-lookup"><span data-stu-id="29c3a-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="29c3a-104">Uporabite [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) da zamenjate mesto mesto z drugim mestom med arhiviranjem na izvirno mesto.</span><span class="sxs-lookup"><span data-stu-id="29c3a-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="29c3a-105">Na voljo za mesto ekipe (ne povezani skupini) in komunikacija stran.</span><span class="sxs-lookup"><span data-stu-id="29c3a-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="29c3a-106">Ne brišite vaše klasične korensko mesto ustvariti mesto sodobne komunikacije.</span><span class="sxs-lookup"><span data-stu-id="29c3a-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="29c3a-107">To je ne podpira Microsoft.</span><span class="sxs-lookup"><span data-stu-id="29c3a-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="29c3a-108">Brisanje korenskega mesta bo vsa SharePointova mesta v organizaciji nedostopen za vse uporabnike, dokler obnovitev mesta ali ustvarite novo mesto na istem spletnem naslovu.</span><span class="sxs-lookup"><span data-stu-id="29c3a-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="29c3a-109">Mi bomo komuniciranje lahk prek centra za sporoèila.</span><span class="sxs-lookup"><span data-stu-id="29c3a-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="29c3a-110">Vi should slutiti zunanja oblika v obstati obrnjen naprej v vaš najemnik kmalu.</span><span class="sxs-lookup"><span data-stu-id="29c3a-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="29c3a-111">Znane težave z zamenjavo strani</span><span class="sxs-lookup"><span data-stu-id="29c3a-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="29c3a-112">Ciljno mesto lahko vrne "not found" napaka (HTTP 404) za kratek čas.</span><span class="sxs-lookup"><span data-stu-id="29c3a-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="29c3a-113">Vsebino morate recrawled želite posodobiti kazalo iskanja.</span><span class="sxs-lookup"><span data-stu-id="29c3a-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="29c3a-114">Ni noben priročnik korak zahteva tukaj, to hoteti obstati velja automatically.</span><span class="sxs-lookup"><span data-stu-id="29c3a-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="29c3a-115">Vse, kar je odvisno od "statična" povezave (na primer datoteka sinhronizacijo in OneNote datoteke) morali ročno popraviti.</span><span class="sxs-lookup"><span data-stu-id="29c3a-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="29c3a-116">Projekt strežnika straneh morda morali potrditi, da se zagotovi, da so še vedno povezani pravilno.</span><span class="sxs-lookup"><span data-stu-id="29c3a-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
