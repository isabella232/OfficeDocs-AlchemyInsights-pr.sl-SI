---
title: Ustvariti spletno stran v SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199289"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="c07c0-102">Ustvarite SharePointova mesta z uporabo predloge</span><span class="sxs-lookup"><span data-stu-id="c07c0-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="c07c0-103">Predloge za mesta SharePoint so ustvarjenimi opredelitve zasnovana okoli za določeno poslovno potrebo.</span><span class="sxs-lookup"><span data-stu-id="c07c0-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="c07c0-104">Če želite več informacij, glejte [Uporaba predloge za ustvarjanje različnih vrst SharePointovih mest](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="c07c0-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="c07c0-105">Tukaj je nekaj pogosta vprašanja/rešitev glede varčevanja je mesto ali seznam kot predlogo v Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="c07c0-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="c07c0-106">**Shrani seznam mest/svetišče popek ni na voljo ali manjka**</span><span class="sxs-lookup"><span data-stu-id="c07c0-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="c07c0-107">Skrbniki morali dovoliti skript po meri omogočiti funkcije predlog.</span><span class="sxs-lookup"><span data-stu-id="c07c0-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c07c0-108">Podrobna navodila, primeri in premisleki najdete</span><span class="sxs-lookup"><span data-stu-id="c07c0-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="c07c0-109">Dovolite ali prepreèite skript po meri</span><span class="sxs-lookup"><span data-stu-id="c07c0-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="c07c0-110">Shrani stran kot predlogo ukaz ni podprt in lahko povzroči težave na mestih, ki uporabljajo SharePoint Server Publishing infrastrukture.</span><span class="sxs-lookup"><span data-stu-id="c07c0-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="c07c0-111">**Predloga mesta ni mogoče ustvariti ali ne deluje pravilno**</span><span class="sxs-lookup"><span data-stu-id="c07c0-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="c07c0-112">Predlogo lahko manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in ne vključite.</span><span class="sxs-lookup"><span data-stu-id="c07c0-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="c07c0-113">Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predlogo mesta ustvariti spletno stran.</span><span class="sxs-lookup"><span data-stu-id="c07c0-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="c07c0-114">Preverite, če vse sezname ali knjižnice presega [Omejitev prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 artiklov, kot to lahko preprečijo nastanek predlogo mesta.</span><span class="sxs-lookup"><span data-stu-id="c07c0-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="c07c0-115">Stran morda uporabljate preveč sredstev in zato predlogo mesta presega omejitev 50 MB.</span><span class="sxs-lookup"><span data-stu-id="c07c0-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="c07c0-116">Obstajajo težave prikazovanje podatkov s seznama, ki uporablja stolpec za iskanje.</span><span class="sxs-lookup"><span data-stu-id="c07c0-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c07c0-117">Če želite več informacij, glejte [Ustvari predlogo seznama ne prikazujejo podatke iz pravilno iskalni seznam v SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="c07c0-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="c07c0-118">Podrobnejše informacije o skupnih problemov in rešitve, si oglejte [Ustvarjanje in uporabo predloge mest](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="c07c0-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



