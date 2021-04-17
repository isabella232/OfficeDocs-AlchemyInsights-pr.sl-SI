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
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818484"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="41987-102">Spreminjanje zahteve za krepka gesla</span><span class="sxs-lookup"><span data-stu-id="41987-102">Change strong password requirement</span></span>

<span data-ttu-id="41987-103">Microsoft privzeto zahteva močna gesla.</span><span class="sxs-lookup"><span data-stu-id="41987-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="41987-104">S storitvijo PowerShell lahko onemogočite močna gesla za določene uporabnike s temi ukazi:</span><span class="sxs-lookup"><span data-stu-id="41987-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="41987-105">Če želite onemogočiti močna gesla za vse uporabnike, uporabite:</span><span class="sxs-lookup"><span data-stu-id="41987-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="41987-106">Več informacij o pravilniku za gesla</span><span class="sxs-lookup"><span data-stu-id="41987-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="41987-107">Vzpostavljanje povezave s storitvijo Microsoft 365 z lupino PowerShell</span><span class="sxs-lookup"><span data-stu-id="41987-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="41987-108">Več informacij o ukazih MsolUser v lupini PowerShell</span><span class="sxs-lookup"><span data-stu-id="41987-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
