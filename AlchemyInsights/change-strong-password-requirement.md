---
title: Spreminjanje zahteve za krepka gesla
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070700"
---
# <a name="change-strong-password-requirement"></a>Spreminjanje zahteve za krepka gesla

Microsoft privzeto zahteva močna gesla.

S storitvijo PowerShell lahko onemogočite močna gesla za določene uporabnike s temi ukazi:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Če želite onemogočiti močna gesla za vse uporabnike, uporabite:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Več informacij o pravilniku za gesla](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Vzpostavljanje povezave z Microsoft 365 z lupino PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Več informacij o ukazih MsolUser v lupini PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
