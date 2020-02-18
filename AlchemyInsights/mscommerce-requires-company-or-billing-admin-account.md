---
title: Vzpostavljanje povezave z modulom MSCommerce
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093632"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="04c87-102">MSCommerce zahteva račun skrbnika podjetja ali računa za obračunavanje</span><span class="sxs-lookup"><span data-stu-id="04c87-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="04c87-103">Modul MSCommerce zahteva račun s privilegiji podjetja ali skrbnika za obračunavanje.</span><span class="sxs-lookup"><span data-stu-id="04c87-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="04c87-104">Če prejmete to napako, boste morali znova vzpostaviti povezavo z drugim računom.</span><span class="sxs-lookup"><span data-stu-id="04c87-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

<span data-ttu-id="04c87-105">Če vaš račun nima pravic podjetja ali skrbnika za obračunavanje, se obrnite na skrbnika za IT.</span><span class="sxs-lookup"><span data-stu-id="04c87-105">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
