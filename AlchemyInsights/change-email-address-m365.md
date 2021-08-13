---
title: Spreminjanje e-poštnega naslova skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995638"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Spreminjanje e-poštnega naslova skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams

E-poštni naslov skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams lahko spremenite v [Skrbniškem središču za Microsoft 365](https://admin.microsoft.com/). Izberite skupino, nato pa izberite »@Uredi e-poštni naslov«.

Primarni naslov SMTP za skupino v okolju Microsoft 365 ali aplikacijo Teams lahko spremenite tudi s tem ukazom EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
