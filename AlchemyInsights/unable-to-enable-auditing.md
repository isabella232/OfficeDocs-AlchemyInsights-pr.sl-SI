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
# <a name="unable-to-enable-unified-auditing"></a>Poenotene revizije ni mogoče omogočiti

Ko poskušate omogočiti poenoteno revizijo za svojo organizacijo, se lahko prikaže napaka, podobna tej:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Če želite odpraviti to težavo, sledite tem korakom:

1. [Vzpostavite povezavo z lupino Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Zaženite ta ukaz» cmdlet «:

   ```
   Enable-OrganizationCustomization
   ```

3. Počakajte 60 minut, da se prejšnja nastavitev ne bo uveljavla.

4. Zaženite ta ukaz v PowerShell Exchange Online:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Za dodatne informacije glejte naslednje članke:

- [Povezovanje z lupino Exchange Online PowerShell z uporabo večfaktorskega preverjanja pristnosti](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Vklop ali izklop iskanja dnevnika revizij](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
