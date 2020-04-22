---
title: Spremeni močno geslo zahteva
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
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706577"
---
# <a name="change-strong-password-requirement"></a>Spreminjanje zahteve po trdnem geslu

Microsoft privzeto zahteva zapletena gesla. 

Z uporabo lupine PowerShell lahko onemogočite zapletena gesla za določene uporabnike s tem ukazom:<br>
*Set-MsolUser-UserPrincipalName <UserPrincipalName> -strongpasswordzahtevani $FALSE*

- [Več informacij o pravilniku o geslih](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kako povezati z Microsoft 365 z PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Več informacij o ukazih lupine MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
