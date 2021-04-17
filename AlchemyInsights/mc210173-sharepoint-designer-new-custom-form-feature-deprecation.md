---
title: MC210173 – ukinitev funkcije za ustvarjanje obrazcev po meri za SharePoint Designer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831822"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="2540c-102">MC210173 – ukinitev funkcije za ustvarjanje obrazcev po meri za SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="2540c-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="2540c-103">Zaznali smo težavo, ki vpliva na funkcijo storitve SharePoint Designer za [ustvarjanje obrazcev po meri](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) v storitvi SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2540c-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="2540c-104">Po skrbni preiskavi smo ugotovili, da ni znanega popravka za to težavo, zato smo se odločili onemogočiti funkcijo ustvarjanja obrazcev po meri, kar bo začelo veljati v nedeljo, 25. aprila 2020 ob 3:00 h UTC.</span><span class="sxs-lookup"><span data-stu-id="2540c-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="2540c-105">Ta sprememba ne vpliva na zmogljivost urejanja že ustvarjenih obrazcev ali drugih obstoječih funkcij v storitvi SharePoint Online Designer.</span><span class="sxs-lookup"><span data-stu-id="2540c-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="2540c-106">Če so uporabniki po tej spremembi poskusili ustvariti nove obrazce, so morda prejeli napako: »Sprememb seznama ni mogoče shraniti v strežnik«.</span><span class="sxs-lookup"><span data-stu-id="2540c-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="2540c-107">Uporabniki, ki so prej uporabljali zmogljivosti storitve SharePoint Designer za ustvarjanje obrazcev po meri, lahko za to namesto tega uporabijo storitev [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="2540c-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="2540c-108">Storitev PowerApps je preprosto in zmogljivo orodje, ki uporabnikom, ki uporabljajo izkušnjo SharePoint Online Modern, omogoča ustvarjanje in urejanje obrazcev po meri za SharePointove sezname in knjižnice dokumentov neposredno v oknu brskalnika.</span><span class="sxs-lookup"><span data-stu-id="2540c-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="2540c-109">Storitev PowerApps ne zahteva dodatnega znanja kodiranja ali dodatnih prenosov aplikacij, kot je InfoPath.</span><span class="sxs-lookup"><span data-stu-id="2540c-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="2540c-110">**Opomba**: uporabniki storitve SharePoint Online Classic bodo morali začasno preklopiti na sodobno izkušnjo, če bodo želeli dostopati do storitve PowerApps in jo uporabljati. Vsi obrazci po meri, ustvarjeni v storitvi PowerApps, pa so dostopni za uporabnike izkušnje SharePoint Online Classic.</span><span class="sxs-lookup"><span data-stu-id="2540c-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
