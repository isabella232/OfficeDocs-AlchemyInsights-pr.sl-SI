---
title: Upokojitev za dostop do storitev
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747801"
---
# <a name="access-services-retirement"></a><span data-ttu-id="3fab1-102">Upokojitev za dostop do storitev</span><span class="sxs-lookup"><span data-stu-id="3fab1-102">Access services retirement</span></span>

<span data-ttu-id="3fab1-103">Kot smo sprva napovedala v MC97576, marec 2017, in še naprej komunicirati v zadnjem letu Access Services so upokojeni iz urada 365.</span><span class="sxs-lookup"><span data-stu-id="3fab1-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="3fab1-104">Naslednja faza v tem procesu bo odstranitev Accessove spletne zbirke podatkov, ki uporabljajo SharePointove sezname kot osnovno shrambo podatkov.</span><span class="sxs-lookup"><span data-stu-id="3fab1-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="3fab1-105">**Kako to vpliva name?**</span><span class="sxs-lookup"><span data-stu-id="3fab1-105">**How does this affect me?**</span></span>

<span data-ttu-id="3fab1-106">Začenši junij 2019, bomo prenehali ustvarjanje novih Accessove zbirke podatkov v SharePoint online in zaustavite storitev in vse preostale aplikacije do aprila 2020.</span><span class="sxs-lookup"><span data-stu-id="3fab1-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="3fab1-107">**Kaj moram storiti, da se pripravim na to spremembo?**</span><span class="sxs-lookup"><span data-stu-id="3fab1-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="3fab1-108">Spodbujamo vas, da ustvarite prehodni načrt za Accessove spletne zbirke podatkov organizacije.</span><span class="sxs-lookup"><span data-stu-id="3fab1-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="3fab1-109">Skrbniki lahko s [skenerjem aplikacije SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pridobijo popis Accessove aplikacije, ki jih uporabljajo spletna mesta.</span><span class="sxs-lookup"><span data-stu-id="3fab1-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="3fab1-110">Podatke Accessove spletne zbirke podatkov lahko preselite na več načinov:</span><span class="sxs-lookup"><span data-stu-id="3fab1-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="3fab1-111">Uvoz v lokalno Accessovo zbirko podatkov (. ACCDB) ali v Excelovo datoteko.</span><span class="sxs-lookup"><span data-stu-id="3fab1-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="3fab1-112">Priporočamo tudi raziskovanje Microsoft PowerApps kot alternativne platforme za ustvarjanje brez kode poslovnih rešitev za spletne in mobilne naprave.</span><span class="sxs-lookup"><span data-stu-id="3fab1-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>