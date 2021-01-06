---
title: Spreminjanje e-poštnega naslova skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756573"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Spreminjanje e-poštnega naslova skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams

E-poštni naslov skupine v okolju Microsoft 365 ali aplikacije Microsoft Teams lahko spremenite v [Skrbniškem središču za Microsoft 365](https://admin.microsoft.com/). Izberite skupino, nato pa izberite »@Uredi e-poštni naslov«.

Primarni naslov SMTP za skupino v okolju Microsoft 365 ali aplikacijo Teams lahko spremenite tudi s tem ukazom EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
