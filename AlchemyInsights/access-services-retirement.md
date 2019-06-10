---
title: Dostop do storitve upokojitev
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769474"
---
# <a name="access-services-retirement"></a><span data-ttu-id="2dd23-102">Dostop do storitve upokojitev</span><span class="sxs-lookup"><span data-stu-id="2dd23-102">Access services retirement</span></span>

<span data-ttu-id="2dd23-103">Kot smo prvotno v MC97576, napovedala v marec 2017, in še naprej komunicirati v preteklem letu so se storitve dostopa upokojeni iz Office 365.</span><span class="sxs-lookup"><span data-stu-id="2dd23-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="2dd23-104">V naslednji fazi v tem procesu bo odstranitev dostop do spletne zbirke podatkov, ki uporabljajo seznami SharePoint kot svoje osnovno shranjevanje podatkov.</span><span class="sxs-lookup"><span data-stu-id="2dd23-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="2dd23-105">**Kako to vpliva na mene?**</span><span class="sxs-lookup"><span data-stu-id="2dd23-105">**How does this affect me?**</span></span>

<span data-ttu-id="2dd23-106">Začetek junija 2019, bomo ustaviti ustvarjanje nove Accessove zbirke podatkov v SharePoint Online in zaustavite storitev in vse preostale apps 2020 aprila.</span><span class="sxs-lookup"><span data-stu-id="2dd23-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="2dd23-107">**Kaj moram storiti, da pripravi spremembe?**</span><span class="sxs-lookup"><span data-stu-id="2dd23-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="2dd23-108">Vas prosimo, da ustvarite načrt prehoda za vaše organizacije dostop do spletne zbirke podatkov.</span><span class="sxs-lookup"><span data-stu-id="2dd23-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="2dd23-109">Administratorji lahko uporabljajo [SharePoint dostop app skener](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pridobiti popis dostop aplikacije, ki uporabljajo mesta.</span><span class="sxs-lookup"><span data-stu-id="2dd23-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="2dd23-110">Obstaja več načinov za selitev dostop spletne podatkovne zbirke podatkov:</span><span class="sxs-lookup"><span data-stu-id="2dd23-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="2dd23-111">Uvoz v lokalni Accessovo zbirko podatkov (. ACCDB) ali Excelovo datoteko.</span><span class="sxs-lookup"><span data-stu-id="2dd23-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="2dd23-112">Priporočamo tudi, da raziskuje Microsoft PowerApps kot alternativna platforma za ustvarjanje brez kode poslovnih rešitev za spletne in mobilne naprave.</span><span class="sxs-lookup"><span data-stu-id="2dd23-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>