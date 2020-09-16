---
title: 2419 – ni mogoče omogočiti nadzora
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
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767615"
---
# <a name="unable-to-enable-unified-auditing"></a>Ni mogoče omogočiti poenotenega nadzora

Ko poskušate omogočiti enotno nadzorovanje organizacije, se lahko prikaže sporočilo o napaki, podobno temu:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Če želite odpraviti to težavo, upoštevajte ta navodila:

1. [Vzpostavite povezavo s storitvijo PowerShell Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Zaženite ta ukaz» cmdlet «:

   ```
   Enable-OrganizationCustomization
   ```

3. Počakajte 60 minut, da se prejšnja nastavitev začne veljati.

4. Zaženite ta ukaz v storitvi Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Če želite več informacij, glejte te članke:

- [Vzpostavljanje povezave s storitvijo PowerShell Exchange Online z več dejavniki preverjanja pristnosti](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Vklop ali izklop iskanja dnevnika nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
