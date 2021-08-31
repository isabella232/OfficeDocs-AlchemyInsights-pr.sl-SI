---
title: User picture not showing in Microsoft Teams organization chart
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792886"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>User picture not showing in Microsoft Teams organization chart

Če eden ali več posameznikov v organizaciji v organigramu manjka njihova fotografija profila, je nastavitev **ShowInAddressLists** morda nastavljena na **False:**

1. Odprite Skrbniško središče za Microsoft 365 > uporabnikov [**in**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)izberite uporabnika, ki ima manjkajočo fotografijo. 
1. Izberite **zavihek** Pošta in preverite, ali je **možnost Pokaži na globalnem seznamu** naslovov nastavljena na **Da.** 

Če nastavitev **ShowInAddressLists** na **Da** ne deluje, preverite to:

- Uporabnik je morda skrit na seznamu prejemnikov v Exchange. Če želite več informacij, [glejte Upravljanje seznamov naslovov v Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Uporabnik je morda skrit na seznamu naslovov v Azure Active Directory. Če želite več informacij, [glejte Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
