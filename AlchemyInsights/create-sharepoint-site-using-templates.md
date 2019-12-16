---
title: Ustvarjanje spletnega mesta v SharePointu online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052485"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="cc02f-102">Ustvarjanje SharePointovih mest s predlogami</span><span class="sxs-lookup"><span data-stu-id="cc02f-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="cc02f-103">SharePointove predloge mest so vnaprej zgrajene definicije, zasnovane za določeno poslovno potrebo.</span><span class="sxs-lookup"><span data-stu-id="cc02f-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="cc02f-104">Če želite več informacij, glejte [Uporaba predlog za ustvarjanje različnih vrst SharePointovih mest](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="cc02f-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="cc02f-105">Tukaj je nekaj pogostih težav/rešitev v zvezi s shranjevanjem mesta ali seznama kot predloge v programu SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="cc02f-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="cc02f-106">**Gumb» Shrani predlogo mesta/seznama «ni na voljo ali manjka**</span><span class="sxs-lookup"><span data-stu-id="cc02f-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="cc02f-107">Skrbniki bodo morali dovoliti skript po meri za omogočanje funkcij predloge.</span><span class="sxs-lookup"><span data-stu-id="cc02f-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="cc02f-108">Za podrobnejše korake, primere in premisleke glej</span><span class="sxs-lookup"><span data-stu-id="cc02f-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="cc02f-109">Omogočanje ali preprečevanje skripta po meri</span><span class="sxs-lookup"><span data-stu-id="cc02f-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="cc02f-110">Ukaz» Shrani mesto kot predlogo «ni podprt in lahko povzroči težave na spletnih mestih, ki uporabljajo infrastrukturo za objavljanje strežnika SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="cc02f-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="cc02f-111">**Predloge mesta ni mogoče ustvariti ali pa ne deluje pravilno**</span><span class="sxs-lookup"><span data-stu-id="cc02f-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="cc02f-112">Predloga morda manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in se ne bo aktivirala.</span><span class="sxs-lookup"><span data-stu-id="cc02f-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="cc02f-113">Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predloge mesta za ustvarjanje mesta.</span><span class="sxs-lookup"><span data-stu-id="cc02f-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="cc02f-114">Preverite, ali seznami ali knjižnice presegajo [prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) za 5000 elementov, saj lahko to blokira ustvarjanje predloge mesta.</span><span class="sxs-lookup"><span data-stu-id="cc02f-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="cc02f-115">Spletna stran lahko uporablja preveč sredstev in zato predlogo mesta presega 50 MB omejitev.</span><span class="sxs-lookup"><span data-stu-id="cc02f-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="cc02f-116">Na seznamu so težave s prikazom podatkov s seznama, ki uporablja stolpec za iskanje.</span><span class="sxs-lookup"><span data-stu-id="cc02f-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="cc02f-117">Če želite več informacij, glejte [predloge-ustvarjeni seznam ne prikaže podatkov s pravilnega seznama za iskanje v SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="cc02f-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="cc02f-118">Za podrobnejše informacije o pogostih problemih in rešitvah preverite [Ustvarjanje in uporabo predlog mesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="cc02f-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



