---
title: 2419-more-za-usposobiti-nadzor
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065705"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="7dff1-102">Ni mogoče usposobiti, enoten nadzor</span><span class="sxs-lookup"><span data-stu-id="7dff1-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="7dff1-103">Ko poskusite omogočiti enotno revidiranja v organizaciji Office 365, lahko dobite sporočilo naslednje:</span><span class="sxs-lookup"><span data-stu-id="7dff1-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="7dff1-104">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="7dff1-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="7dff1-105">[Povezavo za izmenjavo Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="7dff1-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="7dff1-106">Zaženite naslednji ukaz cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7dff1-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="7dff1-107">Čakati na 60 minut za prejšnjo nastavitev začne veljati.</span><span class="sxs-lookup"><span data-stu-id="7dff1-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="7dff1-108">V Exchange Online PowerShell zaženite ta ukaz:</span><span class="sxs-lookup"><span data-stu-id="7dff1-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="7dff1-109">Za dodatne informacije, glejte te članke:</span><span class="sxs-lookup"><span data-stu-id="7dff1-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="7dff1-110">Povezavo z Exchange Online PowerShell uporablja preverjanje pristnosti multifaktorske</span><span class="sxs-lookup"><span data-stu-id="7dff1-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="7dff1-111">Office 365 revizije dnevnik Išči Vklop ali izklop</span><span class="sxs-lookup"><span data-stu-id="7dff1-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
