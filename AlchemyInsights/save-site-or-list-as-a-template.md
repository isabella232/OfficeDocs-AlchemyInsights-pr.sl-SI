---
title: Shranjevanje mesta ali seznama kot predloge
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727547"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="e6a69-102">Shranjevanje mesta ali seznama kot predloge</span><span class="sxs-lookup"><span data-stu-id="e6a69-102">Save site or list as a template</span></span>

<span data-ttu-id="e6a69-103">Predloge SharePointovih mest so vnaprej ustvarjene definicije, oblikovane okoli določene poslovne potrebe.</span><span class="sxs-lookup"><span data-stu-id="e6a69-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="e6a69-104">Če želite več informacij, glejte [Uporaba predlog za ustvarjanje različnih vrst SharePointovih mest](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="e6a69-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="e6a69-105">Tukaj je nekaj pogostih težav/rešitev glede shranjevanja mesta ali seznama kot predloge v SharePoint Onlineu.</span><span class="sxs-lookup"><span data-stu-id="e6a69-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="e6a69-106">**Gumb» Shrani mesto/seznam «ni na voljo ali manjka**.</span><span class="sxs-lookup"><span data-stu-id="e6a69-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="e6a69-107">Skrbniki bodo morali omogočiti skript po meri, če želite omogočiti funkcije predloge.</span><span class="sxs-lookup"><span data-stu-id="e6a69-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="e6a69-108">Če želite podrobna navodila, primeri in premisleki, glejte [Omogočanje ali preprečevanje skripta po meri](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="e6a69-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="e6a69-109">Ukaz» Shrani mesto kot predlogo «ni podprt in lahko povzroči težave na mestih, ki uporabljajo SharePoint Server Publishing Infrastructure.</span><span class="sxs-lookup"><span data-stu-id="e6a69-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="e6a69-110">**Predloge mesta ni mogoče ustvariti ali pa ne deluje pravilno**</span><span class="sxs-lookup"><span data-stu-id="e6a69-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="e6a69-111">Predloga morda manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in ne bo aktivirana.</span><span class="sxs-lookup"><span data-stu-id="e6a69-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="e6a69-112">Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predloge mesta za ustvarjanje spletnega mesta.</span><span class="sxs-lookup"><span data-stu-id="e6a69-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="e6a69-113">Preverite, ali kateri koli seznami ali knjižnice presegajo [mejni prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) v 5000 elementih, saj lahko to blokira ustvarjanje predloge mesta.</span><span class="sxs-lookup"><span data-stu-id="e6a69-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="e6a69-114">Mesto lahko uporablja preveč virov in zato predloga mesta presega omejitev 50 megabajtov (MB).</span><span class="sxs-lookup"><span data-stu-id="e6a69-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="e6a69-115">Na voljo so težave s prikazom podatkov s seznama, ki uporablja stolpec za iskanje.</span><span class="sxs-lookup"><span data-stu-id="e6a69-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="e6a69-116">Če želite več informacij, glejte [seznam ustvarjenih predlog ne prikazuje podatkov s pravilnega seznama za iskanje v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="e6a69-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="e6a69-117">Če želite podrobnejše informacije o pogostih težavah in rešitvah, se lahko sklicujete na [Ustvarjanje in uporabo predlog spletnega mesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="e6a69-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

