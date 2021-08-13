---
title: 2419 –ni mogoče omogočiti nadzora
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007806"
---
# <a name="unable-to-enable-unified-auditing"></a>Poenotenega nadzora ni mogoče omogočiti

Ko poskušate omogočiti poenoten nadzor za svojo organizacijo, se lahko prikaže sporočilo o napaki, podobno tej:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Če želite odpraviti to težavo, upoštevajte ta navodila:

1. [Povezovalnik, da Exchange Online Powershell.](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)

2. Zaženite ta ukaz »cmdlet«:

   ```
   Enable-OrganizationCustomization
   ```

3. Počakajte 60 minut, da začne veljati prejšnja nastavitev.

4. V lupini PowerShell zaženite Exchange Online ukaz:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Dodatne informacije najdete v teh člankih:

- [Povezovalnik večkratnega preverjanja Exchange Online večkratnega preverjanja pristnosti za PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Vklop ali izklop iskanja v dnevniku nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
