---
title: 2419-ne morem-v-usposobiti-revidiranje
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510444"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="7b9cf-102">Poenotene revizije ni mogoče omogočiti</span><span class="sxs-lookup"><span data-stu-id="7b9cf-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="7b9cf-103">Ko poskušate omogočiti poenoteno revizijo za svojo organizacijo, se lahko prikaže napaka, podobna tej:</span><span class="sxs-lookup"><span data-stu-id="7b9cf-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="7b9cf-104">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="7b9cf-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="7b9cf-105">[Vzpostavite povezavo z lupino Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="7b9cf-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="7b9cf-106">Zaženite ta ukaz» cmdlet «:</span><span class="sxs-lookup"><span data-stu-id="7b9cf-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="7b9cf-107">Počakajte 60 minut, da se prejšnja nastavitev ne bo uveljavla.</span><span class="sxs-lookup"><span data-stu-id="7b9cf-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="7b9cf-108">Zaženite ta ukaz v PowerShell Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="7b9cf-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="7b9cf-109">Za dodatne informacije glejte naslednje članke:</span><span class="sxs-lookup"><span data-stu-id="7b9cf-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="7b9cf-110">Povezovanje z lupino Exchange Online PowerShell z uporabo večfaktorskega preverjanja pristnosti</span><span class="sxs-lookup"><span data-stu-id="7b9cf-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="7b9cf-111">Vklop ali izklop iskanja dnevnika revizij</span><span class="sxs-lookup"><span data-stu-id="7b9cf-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
