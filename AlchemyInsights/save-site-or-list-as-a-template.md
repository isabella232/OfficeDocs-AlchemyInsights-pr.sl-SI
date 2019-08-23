---
title: Shraniti stran ali seznam kot predlogo
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551647"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="e53e9-102">Shraniti stran ali seznam kot predlogo</span><span class="sxs-lookup"><span data-stu-id="e53e9-102">Save site or list as a template</span></span>

<span data-ttu-id="e53e9-103">Predloge za mesta SharePoint so ustvarjenimi opredelitve zasnovana okoli za določeno poslovno potrebo.</span><span class="sxs-lookup"><span data-stu-id="e53e9-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="e53e9-104">Če želite več informacij, glejte [Uporaba predloge za ustvarjanje različnih vrst SharePointovih mest](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="e53e9-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="e53e9-105">Tukaj je nekaj pogosta vprašanja/rešitev glede varčevanja je mesto ali seznam kot predlogo v SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="e53e9-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="e53e9-106">**Shrani seznam mest/svetišče popek je ni na voljo ali pa manjka**.</span><span class="sxs-lookup"><span data-stu-id="e53e9-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="e53e9-107">Skrbniki morali dovoliti skript po meri omogočiti funkcije predlog.</span><span class="sxs-lookup"><span data-stu-id="e53e9-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="e53e9-108">Podrobni koraki, primeri in vidiki glejte [Dovoli ali prepreči skript po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e53e9-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="e53e9-109">Shrani stran kot predlogo ukaz ni podprt in lahko povzroči težave na mestih, ki uporabljajo SharePoint Server Publishing infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="e53e9-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="e53e9-110">**Predloga mesta ni mogoče ustvariti ali ne deluje pravilno**</span><span class="sxs-lookup"><span data-stu-id="e53e9-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="e53e9-111">Predlogo lahko manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in ne vključite.</span><span class="sxs-lookup"><span data-stu-id="e53e9-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="e53e9-112">Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predlogo mesta ustvariti spletno stran.</span><span class="sxs-lookup"><span data-stu-id="e53e9-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="e53e9-113">Preverite, če vse sezname ali knjižnice presega [Omejitev prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 artiklov, kot to lahko preprečijo nastanek predlogo mesta.</span><span class="sxs-lookup"><span data-stu-id="e53e9-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="e53e9-114">Stran morda uporabljate preveč sredstev in zato predlogo mesta presega omejitev 50 megabajtov (MB).</span><span class="sxs-lookup"><span data-stu-id="e53e9-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="e53e9-115">Obstajajo težave prikazovanje podatkov s seznama, ki uporablja stolpec za iskanje.</span><span class="sxs-lookup"><span data-stu-id="e53e9-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="e53e9-116">Če želite več informacij, glejte [Ustvari predlogo seznama ne prikazujejo podatke iz pravilno iskalni seznam v SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="e53e9-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="e53e9-117">Za podrobnejše informacije o skupnih problemov in rešitve vas prosimo, reference, [Ustvarjanje in uporabo predloge mest](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="e53e9-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

