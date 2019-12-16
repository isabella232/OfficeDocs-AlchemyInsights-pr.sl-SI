---
title: Elementov v SharePointu ali storitvi OneDrive ni mogoče izbrisati
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049533"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="84dbe-102">Elementov ni mogoče izbrisati</span><span class="sxs-lookup"><span data-stu-id="84dbe-102">Unable to delete items</span></span>

<span data-ttu-id="84dbe-103">Imate težave pri brisanju SharePointovih elementov?</span><span class="sxs-lookup"><span data-stu-id="84dbe-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="84dbe-104">Vedno se prepričajte, da imate [ustrezna dovoljenja](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) za izbris elementa ali pa je [skrbnik zbirke mest](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) poskušal odstraniti element.</span><span class="sxs-lookup"><span data-stu-id="84dbe-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="84dbe-105">Zagotovite, da na elementu ni nastavitve [pravilnika o hranjenju](https://docs.microsoft.com/office365/securitycompliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="84dbe-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="84dbe-106">Zagotovite, da element ni [rezerviran](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugemu uporabniku.</span><span class="sxs-lookup"><span data-stu-id="84dbe-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="84dbe-107">Nazadnje skrbniki lahko uporabljajo [SharePointove vzorce in prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ki vsebujejo knjižnico ukazov PowerShell, ki vam omogočajo izvajanje zapletenih dejanj upravljanja, kot je vsiliti brisanje trdovratnih elementov.</span><span class="sxs-lookup"><span data-stu-id="84dbe-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="84dbe-108">Odstrani datoteko PNP</span><span class="sxs-lookup"><span data-stu-id="84dbe-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="84dbe-109">Odstrani mapo PNP</span><span class="sxs-lookup"><span data-stu-id="84dbe-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="84dbe-110">Odstrani element seznama PNP</span><span class="sxs-lookup"><span data-stu-id="84dbe-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="84dbe-111">Odstrani seznam PNP</span><span class="sxs-lookup"><span data-stu-id="84dbe-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="84dbe-112">Odstrani PNP polje (stolpec)</span><span class="sxs-lookup"><span data-stu-id="84dbe-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)