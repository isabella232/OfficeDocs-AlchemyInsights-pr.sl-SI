---
title: Spreminjanje e-poštnega naslova skupine Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580673"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Spreminjanje e-poštnega naslova skupine Microsoft 365

E-poštni naslov skupine Microsoft 365 lahko spremenite s skrbniškim središčem. Samo izberite skupino in izberite @edit e-poštni naslov.

Če želite spremeniti primarni naslov SMTP skupine Microsoft 365, lahko uporabite tudi naslednje ukaze EXO PowerShell:

Set-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address>

Primer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
