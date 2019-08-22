---
title: Sprememba zahteva močno geslo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518775"
---
# <a name="change-strong-password-requirement"></a>Sprememba zahteva močno geslo

Microsoft zahteva močnih gesel, privzeto. 

Z uporabo PowerShell, lahko onemogočite močnih gesel za določene uporabnike, s tem ukazom:<br>
*Set-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Če želite več informacij o politiki geslo](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kako povezati Office 365 v PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Več informacij o PowerShell MsolUser ukaze](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)