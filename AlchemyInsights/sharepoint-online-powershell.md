---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830598"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="37887-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="37887-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="37887-103">Ali delate z lupino PowerShell ali skripti v SharePoint Onlineu?</span><span class="sxs-lookup"><span data-stu-id="37887-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="37887-104">Več informacij najdete na spodnjih povezavah.</span><span class="sxs-lookup"><span data-stu-id="37887-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="37887-105">Uvod v ukazno lupino storitve SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="37887-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="37887-106">Vzpostavljanje povezave z lupino SPO PowerShell z večkratnikom preverjanja pristnosti (MFA)</span><span class="sxs-lookup"><span data-stu-id="37887-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="37887-107">[V SharePointovih vzorcih in praksah (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) je knjižnica ukazov ogrodja PowerShell, s katerim lahko izvajate zapletena dejanja upravljanja v zvezi s SharePointom.</span><span class="sxs-lookup"><span data-stu-id="37887-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="37887-108">Če imate težave s povezovanjem z lupino za upravljanje SPO, se [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) prepričajte, da ste posodobili na najnovejšo različico, in poskusite modul znova uvoziti z ukazom *»Import-Module Microsoft.Online.SharePoint.PowerShell«.*</span><span class="sxs-lookup"><span data-stu-id="37887-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="37887-109">Če poskušate zagnati skripte odjemalskega predmetnega modela, morate imeti v lokalnem računalniku nameščene komponente [odjemalskega SDK za Sharepoint Online.](https://www.microsoft.com/download/details.aspx?id=42038)</span><span class="sxs-lookup"><span data-stu-id="37887-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="37887-110">Če imate težave pri zagonu skriptov iz lupine PowerShell, vam je morda najbolje, da zaženete PowerShell kot skrbnik in spremenite pravilnik [za izvajanje.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)</span><span class="sxs-lookup"><span data-stu-id="37887-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>