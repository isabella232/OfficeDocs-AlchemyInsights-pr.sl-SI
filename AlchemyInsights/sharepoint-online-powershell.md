---
title: Spletna PowerShell za SharePoint online
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764277"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="4bd6c-102">Spletna PowerShell za SharePoint online</span><span class="sxs-lookup"><span data-stu-id="4bd6c-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="4bd6c-103">Delo z PowerShell ali skripte v SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="4bd6c-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="4bd6c-104">Za več informacij obiščite spodnje povezave.</span><span class="sxs-lookup"><span data-stu-id="4bd6c-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="4bd6c-105">Uvod v SharePoint online Management Shell</span><span class="sxs-lookup"><span data-stu-id="4bd6c-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="4bd6c-106">Vzpostavljanje povezave z lupino SPO PowerShell z večfaktorskega preverjanja pristnosti (MFA)</span><span class="sxs-lookup"><span data-stu-id="4bd6c-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="4bd6c-107">[SharePointovi vzorci in prakse (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) vsebujejo knjižnico ukazov PowerShell, ki vam omogoča izvajanje zapletenih ukrepov upravljanja proti spo.</span><span class="sxs-lookup"><span data-stu-id="4bd6c-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="4bd6c-108">Če imate težave pri povezovanju z lupino SPO upravljanje, se prepričajte, da ste posodobili na najnovejšo različico in poskusite [ponovno uvoziti modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) z uporabo *"Import-module Microsoft. online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="4bd6c-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="4bd6c-109">Če poskušate zagnati skripte za predmetni model odjemalca, boste morali v lokalnem računalniku imeti nameščen SDK za [komponente odjemalca SharePoint online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="4bd6c-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="4bd6c-110">Če imate težave pri zagonu skriptov iz lupine PowerShell, boste morda želeli razmisliti o zagonu lupine PowerShell kot skrbnika in spreminjanju [pravilnika o izvrševanju](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="4bd6c-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>