---
title: Shranjevanje mesta ali seznama kot predloge
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048740"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="be5d2-102">Shranjevanje mesta ali seznama kot predloge</span><span class="sxs-lookup"><span data-stu-id="be5d2-102">Save site or list as a template</span></span>

<span data-ttu-id="be5d2-103">SharePointove predloge mest so vnaprej zgrajene definicije, zasnovane za določeno poslovno potrebo.</span><span class="sxs-lookup"><span data-stu-id="be5d2-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="be5d2-104">Če želite več informacij, glejte [Uporaba predlog za ustvarjanje različnih vrst SharePointovih mest](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="be5d2-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="be5d2-105">Tukaj je nekaj pogostih težav/rešitev v zvezi s shranjevanjem mesta ali seznama kot predloge v programu SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="be5d2-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="be5d2-106">**Shrani gumb predloge mesta/seznama ni na voljo ali manjka**.</span><span class="sxs-lookup"><span data-stu-id="be5d2-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="be5d2-107">Skrbniki bodo morali dovoliti skript po meri za omogočanje funkcij predloge.</span><span class="sxs-lookup"><span data-stu-id="be5d2-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="be5d2-108">Za podrobnejše korake, primere in premisleke glejte [Omogočanje ali preprečevanje skripta po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="be5d2-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="be5d2-109">Ukaz» Shrani mesto kot predlogo «ni podprt in lahko povzroči težave na spletnih mestih, ki uporabljajo infrastrukturo za objavljanje strežnika SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="be5d2-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="be5d2-110">**Predloge mesta ni mogoče ustvariti ali pa ne deluje pravilno**</span><span class="sxs-lookup"><span data-stu-id="be5d2-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="be5d2-111">Predloga morda manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in se ne bo aktivirala.</span><span class="sxs-lookup"><span data-stu-id="be5d2-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="be5d2-112">Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predloge mesta za ustvarjanje mesta.</span><span class="sxs-lookup"><span data-stu-id="be5d2-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="be5d2-113">Preverite, ali seznami ali knjižnice presegajo [prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) za 5000 elementov, saj lahko to blokira ustvarjanje predloge mesta.</span><span class="sxs-lookup"><span data-stu-id="be5d2-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="be5d2-114">Spletno mesto morda uporablja preveč virov, zato predloga mesta presega omejitev 50 megabajtov (MB).</span><span class="sxs-lookup"><span data-stu-id="be5d2-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="be5d2-115">Na seznamu so težave s prikazom podatkov s seznama, ki uporablja stolpec za iskanje.</span><span class="sxs-lookup"><span data-stu-id="be5d2-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="be5d2-116">Če želite več informacij, glejte [predloge-ustvarjeni seznam ne prikaže podatkov s pravilnega seznama za iskanje v SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="be5d2-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="be5d2-117">Podrobnejše informacije o pogostih problemih in rešitvah so na voljo v temi, [Ustvarjanje in uporaba predlog mesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="be5d2-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

