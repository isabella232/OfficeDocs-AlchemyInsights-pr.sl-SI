---
title: Storitev PowerShell v storitvi SharePoint online
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709086"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="59107-102">Storitev PowerShell v storitvi SharePoint online</span><span class="sxs-lookup"><span data-stu-id="59107-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="59107-103">Ali delate z PowerShellom ali skripti v storitvi SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="59107-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="59107-104">Če želite več informacij, obiščite spodnje povezave.</span><span class="sxs-lookup"><span data-stu-id="59107-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="59107-105">Uvod v ukazno lupino za upravljanje storitve SharePoint online</span><span class="sxs-lookup"><span data-stu-id="59107-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="59107-106">Povezovanje z SPO PowerShell s preverjanjem pristnosti z več dejstvi (MFA)</span><span class="sxs-lookup"><span data-stu-id="59107-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="59107-107">V [SharePointovih vzorcih in praksah (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) je knjižnica ukazov PowerShell, ki omogoča izvajanje zapletenih upravljalnih dejanj za spo.</span><span class="sxs-lookup"><span data-stu-id="59107-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="59107-108">Če imate težave s povezovanjem z lupino za upravljanje SPO, se prepričajte, da ste posodobili najnovejšo različico in poskusite [znova uvoziti modul](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) z uporabo *» Import-modul Microsoft. online. SharePoint. PowerShell «.*</span><span class="sxs-lookup"><span data-stu-id="59107-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="59107-109">Če poskušate zagnati skripte za odjemalski predmetni model, boste morali imeti v lokalnem računalniku nameščen sistem [SharePoint online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="59107-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="59107-110">Če imate težave z zaganjanjem skriptov iz lupine PowerShell, boste morda želeli razmisliti o zaganjanju lupine PowerShell kot skrbnika in spreminjanju [pravilnika o izvajanju](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="59107-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>