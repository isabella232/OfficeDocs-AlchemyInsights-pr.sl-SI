---
title: Ni mogoče izbrisati elemente v SharePoint ali OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057776"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="d13ea-102">Ni mogoče izbrisati elemente</span><span class="sxs-lookup"><span data-stu-id="d13ea-102">Unable to delete items</span></span>

<span data-ttu-id="d13ea-103">Ob vprašanjih, brisanje elementov?</span><span class="sxs-lookup"><span data-stu-id="d13ea-103">Having issues deleting items?</span></span>

- <span data-ttu-id="d13ea-104">Vedno preverite, ali imate [ustrezna dovoljenja](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) za brisanje elementa ali so [skrbnike](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) poskus, odstranite element.</span><span class="sxs-lookup"><span data-stu-id="d13ea-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="d13ea-105">Zagotoviti, da je ne setup [zadrževanja](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) na element.</span><span class="sxs-lookup"><span data-stu-id="d13ea-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="d13ea-106">Zagotoviti element ni [rezerviran](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) za drugega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="d13ea-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="d13ea-107">Končno, lahko skrbniki [SharePoint vzorce in prakse](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ki vsebuje knjižnico PowerShell ukaze, ki omogočajo izvajanje zapletenih upravljanjem, kot sila izbrisom trmast.</span><span class="sxs-lookup"><span data-stu-id="d13ea-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="d13ea-108">Odstranite datoteko PNP</span><span class="sxs-lookup"><span data-stu-id="d13ea-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="d13ea-109">Odstranite PNP mapo</span><span class="sxs-lookup"><span data-stu-id="d13ea-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="d13ea-110">Odstranite element seznama PNP</span><span class="sxs-lookup"><span data-stu-id="d13ea-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="d13ea-111">Odstranite PNP seznam</span><span class="sxs-lookup"><span data-stu-id="d13ea-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="d13ea-112">Odstranite PNP polju (stolpcu)</span><span class="sxs-lookup"><span data-stu-id="d13ea-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)