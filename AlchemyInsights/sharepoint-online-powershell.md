---
title: Spletna PowerShell za SharePoint online
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123014"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6261b-102">Spletna PowerShell za SharePoint online</span><span class="sxs-lookup"><span data-stu-id="6261b-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6261b-103">Delo z PowerShell ali skripte v SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="6261b-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6261b-104">Za več informacij obiščite spodnje povezave.</span><span class="sxs-lookup"><span data-stu-id="6261b-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6261b-105">Uvod v SharePoint online Management Shell</span><span class="sxs-lookup"><span data-stu-id="6261b-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6261b-106">Vzpostavljanje povezave z lupino SPO PowerShell z večfaktorskega preverjanja pristnosti (MFA)</span><span class="sxs-lookup"><span data-stu-id="6261b-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6261b-107">[SharePointovi vzorci in prakse (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) vsebujejo knjižnico ukazov PowerShell, ki vam omogoča izvajanje zapletenih ukrepov upravljanja proti spo.</span><span class="sxs-lookup"><span data-stu-id="6261b-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6261b-108">Če imate težave pri povezovanju z lupino SPO upravljanje, se prepričajte, da ste posodobili na najnovejšo različico in poskusite [ponovno uvoziti modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) z uporabo *"Import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="6261b-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6261b-109">Če poskušate zagnati skripte za predmetni model odjemalca, boste morali v lokalnem računalniku imeti nameščen SDK za [komponente odjemalca SharePoint online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="6261b-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6261b-110">Če imate težave pri zagonu skriptov iz lupine PowerShell, boste morda želeli razmisliti o zagonu lupine PowerShell kot skrbnika in spreminjanju [pravilnika o izvrševanju](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="6261b-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>