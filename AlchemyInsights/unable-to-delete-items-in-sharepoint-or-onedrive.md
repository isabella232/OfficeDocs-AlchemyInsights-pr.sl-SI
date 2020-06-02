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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511992"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="3f35f-102">Elementov ni mogoče izbrisati</span><span class="sxs-lookup"><span data-stu-id="3f35f-102">Unable to delete items</span></span>

<span data-ttu-id="3f35f-103">Pravilniki o hranjenju lahko povzročijo to, zato morate onemogočiti ali izključiti ustrezno zadržanje, ki povzroča to težavo.</span><span class="sxs-lookup"><span data-stu-id="3f35f-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="3f35f-104">Ko je pravilnik o hranjenju ali zadržanje odstranjen, lahko traja do 24 ur, da sprememba učinkuje.</span><span class="sxs-lookup"><span data-stu-id="3f35f-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="3f35f-105">Zagotovite, da na elementu ni nastavitve [pravilnika o hranjenju](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="3f35f-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="3f35f-106">Mesto je morda preseglo omejitev shranjevanja, povečalo [kvoto mesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) in zbrisal element.</span><span class="sxs-lookup"><span data-stu-id="3f35f-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="3f35f-107">Zagotovite, da element ni [rezerviran](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) drugemu uporabniku.</span><span class="sxs-lookup"><span data-stu-id="3f35f-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="3f35f-108">Nazadnje skrbniki lahko uporabljajo [SharePointove vzorce in prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ki vsebujejo knjižnico ukazov PowerShell, ki vam omogočajo izvajanje zapletenih dejanj upravljanja, kot je vsiliti brisanje trdovratnih elementov.</span><span class="sxs-lookup"><span data-stu-id="3f35f-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="3f35f-109">Odstrani datoteko PNP</span><span class="sxs-lookup"><span data-stu-id="3f35f-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="3f35f-110">Odstrani mapo PNP</span><span class="sxs-lookup"><span data-stu-id="3f35f-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="3f35f-111">Odstrani element seznama PNP</span><span class="sxs-lookup"><span data-stu-id="3f35f-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="3f35f-112">Odstrani seznam PNP</span><span class="sxs-lookup"><span data-stu-id="3f35f-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="3f35f-113">Odstrani PNP polje (stolpec)</span><span class="sxs-lookup"><span data-stu-id="3f35f-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)