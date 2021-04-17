---
title: Sprememba e-poštnega naslova skupine v storitvi Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819060"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Sprememba e-poštnega naslova skupine v storitvi Microsoft 365

E-poštni naslov skupine v storitvi Microsoft 365 lahko spremenite v skrbniškem središču. Izberite skupino, nato pa izberite »@Uredi e-poštni naslov«.

Primarni naslov SMTP za skupino v storitvi Microsoft 365 lahko spremenite tudi s sledečim ukazom EXO Windows PowerShell:

Niz-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Primer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
