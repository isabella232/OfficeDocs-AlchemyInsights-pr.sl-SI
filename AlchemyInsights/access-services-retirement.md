---
title: Pokojnine za dostop do storitev
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698698"
---
# <a name="access-services-retirement"></a><span data-ttu-id="0d1bc-102">Pokojnine za dostop do storitev</span><span class="sxs-lookup"><span data-stu-id="0d1bc-102">Access services retirement</span></span>

<span data-ttu-id="0d1bc-103">Kot smo sprva objavili v MC97576, je marca 2017 in nadaljevalo komuniciranje v preteklem letu, ko so se upokojili.</span><span class="sxs-lookup"><span data-stu-id="0d1bc-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="0d1bc-104">Naslednja faza v tem postopku bo odstranitev Accessovih spletnih zbirk podatkov, ki uporabljajo SharePointove sezname kot osnovna shramba podatkov.</span><span class="sxs-lookup"><span data-stu-id="0d1bc-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="0d1bc-105">**Kako to vpliva name?**</span><span class="sxs-lookup"><span data-stu-id="0d1bc-105">**How does this affect me?**</span></span>

<span data-ttu-id="0d1bc-106">Z začetkom junija 2019 bomo ustavili ustvarjanje novih Accessovih zbirk podatkov v storitvi SharePoint online in zaprli storitev ter vse preostale aplikacije do aprila 2020.</span><span class="sxs-lookup"><span data-stu-id="0d1bc-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="0d1bc-107">**Kaj moram narediti, da se pripravim na to spremembo?**</span><span class="sxs-lookup"><span data-stu-id="0d1bc-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="0d1bc-108">Priporočamo vam, da ustvarite načrt prehoda za Accessove spletne zbirke podatkov organizacije.</span><span class="sxs-lookup"><span data-stu-id="0d1bc-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="0d1bc-109">Skrbniki lahko s [skenerjem programa SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) pridobijo seznam Accessovih programov, ki jih uporabljajo spletna mesta.</span><span class="sxs-lookup"><span data-stu-id="0d1bc-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="0d1bc-110">Podatke o Accessovih spletnih zbirkah podatkov lahko preselite na več načinov:</span><span class="sxs-lookup"><span data-stu-id="0d1bc-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="0d1bc-111">Uvoz v lokalno Accessovo zbirko podatkov (. ACCDB) ali v Excelovo datoteko.</span><span class="sxs-lookup"><span data-stu-id="0d1bc-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="0d1bc-112">Priporočamo tudi, da raziskujete Microsoft PowerApps kot alternativno platformo za ustvarjanje poslovnih rešitev brez kode za spletne in prenosne naprave.</span><span class="sxs-lookup"><span data-stu-id="0d1bc-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>