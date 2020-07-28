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
# <a name="unable-to-change-username"></a>Uporabniškega imena ni mogoče spremeniti

V nekaterih primerih se spremembe UPN (UserPrincipalName) ne razširijo v oblak. Napake pri preverjanju veljavnosti se lahko prikažejo na portalu storitve Office 365 ali pa ne morete spremeniti uporabniškega imena ali e-poštnega naslova. Če želite odpraviti to težavo, ročno nastavite UserPrincipalName s tem ukazom PowerShell.

**Primer: Preimenovanje uporabnika**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Ta ukaz preimenuje davidc@contoso.com v davidchew@contoso.com.

Če želite več informacij, [glejte Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).