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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770855"
---
# <a name="sharepoint-online-powershell"></a>Storitev PowerShell v storitvi SharePoint online

Ali delate z PowerShellom ali skripti v storitvi SharePoint online? Če želite več informacij, obiščite spodnje povezave.
- [Uvod v ukazno lupino za upravljanje storitve SharePoint online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Povezovanje z SPO PowerShell s preverjanjem pristnosti z več dejstvi (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- V [SharePointovih vzorcih in praksah (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) je knjižnica ukazov PowerShell, ki omogoča izvajanje zapletenih upravljalnih dejanj za spo.

> [!NOTE]
> - Če imate težave s povezovanjem z lupino za upravljanje SPO, se prepričajte, da ste posodobili najnovejšo različico in poskusite [znova uvoziti modul](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) z uporabo *» Import-modul Microsoft. online. SharePoint. PowerShell «.*
> - Če poskušate zagnati skripte za odjemalski predmetni model, boste morali imeti v lokalnem računalniku nameščen sistem [SharePoint online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) .
> - Če imate težave z zaganjanjem skriptov iz lupine PowerShell, boste morda želeli razmisliti o zaganjanju lupine PowerShell kot skrbnika in spreminjanju [pravilnika o izvajanju](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).