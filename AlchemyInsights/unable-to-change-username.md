---
title: Uporabniškega imena ni mogoče spremeniti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440298"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="a60cd-102">Uporabniškega imena ni mogoče spremeniti</span><span class="sxs-lookup"><span data-stu-id="a60cd-102">Unable to change UserName</span></span>

<span data-ttu-id="a60cd-103">V nekaterih primerih se spremembe UPN (UserPrincipalName) ne razširijo v oblak.</span><span class="sxs-lookup"><span data-stu-id="a60cd-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="a60cd-104">Napake pri preverjanju veljavnosti se lahko prikažejo na portalu storitve Office 365 ali pa ne morete spremeniti uporabniškega imena ali e-poštnega naslova.</span><span class="sxs-lookup"><span data-stu-id="a60cd-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="a60cd-105">Če želite odpraviti to težavo, ročno nastavite UserPrincipalName s tem ukazom PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a60cd-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="a60cd-106">**Primer: Preimenovanje uporabnika**</span><span class="sxs-lookup"><span data-stu-id="a60cd-106">**Example: Rename a user**</span></span>

<span data-ttu-id="a60cd-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="a60cd-107">PowerShellCopy</span></span>

<span data-ttu-id="a60cd-108">PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="a60cd-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="a60cd-109">Ta ukaz preimenuje davidc@contoso.com v davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="a60cd-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="a60cd-110">Če želite več informacij, [glejte Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="a60cd-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>