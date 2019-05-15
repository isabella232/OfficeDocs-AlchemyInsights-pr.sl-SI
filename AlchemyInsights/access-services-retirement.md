---
title: Dostop do storitve upokojitev
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973950"
---
# <a name="access-services-retirement"></a><span data-ttu-id="17541-102">Dostop do storitve upokojitev</span><span class="sxs-lookup"><span data-stu-id="17541-102">Access services retirement</span></span>

<span data-ttu-id="17541-103">Kot smo prvotno v MC97576, napovedala v marec 2017, in še naprej komunicirati v preteklem letu so se storitve dostopa upokojeni iz Office 365.</span><span class="sxs-lookup"><span data-stu-id="17541-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="17541-104">V naslednji fazi v tem procesu bo odstranitev dostop do spletne zbirke podatkov, ki uporabljajo seznami SharePoint kot svoje osnovno shranjevanje podatkov.</span><span class="sxs-lookup"><span data-stu-id="17541-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="17541-105">Kako to vpliva na mene?</span><span class="sxs-lookup"><span data-stu-id="17541-105">How does this affect me?</span></span>

<span data-ttu-id="17541-106">Začetek junija 2019, bomo ustaviti ustvarjanje nove Accessove zbirke podatkov v SharePoint Online in zaustavite storitev in vse preostale apps 2020 aprila.</span><span class="sxs-lookup"><span data-stu-id="17541-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="17541-107">Kaj moram storiti, da pripravi spremembe?</span><span class="sxs-lookup"><span data-stu-id="17541-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="17541-108">Vas prosimo, da ustvarite načrt prehoda za vaše organizacije dostop do spletne zbirke podatkov.</span><span class="sxs-lookup"><span data-stu-id="17541-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="17541-109">Administratorji lahko uporabljajo [SharePoint dostop app skener](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) pridobiti popis dostop aplikacije, ki uporabljajo mesta.</span><span class="sxs-lookup"><span data-stu-id="17541-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="17541-110">Obstaja več načinov za selitev dostop spletne podatkovne zbirke podatkov:</span><span class="sxs-lookup"><span data-stu-id="17541-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="17541-111">Uvoz v lokalni Accessovo zbirko podatkov (. ACCDB) ali Excelovo datoteko.</span><span class="sxs-lookup"><span data-stu-id="17541-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="17541-112">Priporočamo tudi, da raziskuje Microsoft PowerApps kot alternativna platforma za ustvarjanje brez kode poslovnih rešitev za spletne in mobilne naprave.</span><span class="sxs-lookup"><span data-stu-id="17541-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>