---
title: Slika uporabnika je še vedno prikazana v Microsoft Teams organigramu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422318"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Slika uporabnika je še vedno prikazana v Microsoft Teams organigramu

Če je bil eden ali več posameznikov v vaši organizaciji onemogočenih ali odstranjenih in je njihova fotografija profila še vedno prikazana v organigramu, je nastavitev **ShowInAddressLists** morda nastavljena na False: 

1. Pojdite na Skrbniško središče za Microsoft 365 > [aktivnih uporabnikov](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) in izberite uporabnika s fotografijo, ki je še vedno prikazana. 
1. Izberite **zavihek Pošta** in se prepričajte, da je možnost Pokaži na **globalnem seznamu** naslovov nastavljena na **Ne.**

Če nastavitev **ShowInAddressLists** na **Ne** ne deluje, preverite to: 

- Uporabnik je morda prikazan na seznamu prejemnikov v Exchange. Če želite več informacij, [glejte Upravljanje seznamov naslovov v Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Uporabnik je morda prikazan na seznamu naslovov v Azure Active Directory. Če želite več informacij, [glejte Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 