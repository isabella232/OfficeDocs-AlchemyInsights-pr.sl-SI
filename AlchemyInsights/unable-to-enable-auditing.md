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
# <a name="unable-to-enable-unified-auditing"></a>Ni mogoče usposobiti, enoten nadzor

Ko poskusite omogočiti enotno revidiranja v organizaciji Office 365, lahko dobite sporočilo naslednje:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Če želite odpraviti to težavo, sledite tem korakom:

1. [Povezavo za izmenjavo Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Zaženite naslednji ukaz cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Čakati na 60 minut za prejšnjo nastavitev začne veljati.

4. V Exchange Online PowerShell zaženite ta ukaz:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Za dodatne informacije, glejte te članke:

- [Povezavo z Exchange Online PowerShell uporablja preverjanje pristnosti multifaktorske](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 revizije dnevnik Išči Vklop ali izklop](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
