---
title: DLP končne točke ni uveden v uporabnikovo napravo
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731868"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>DLP končne točke ni uveden v uporabnikovo napravo

Če nastavitev za preprečitev izgube podatkov končne točke (DLP) ni uporabljena za uporabnikovo napravo, potrdite, da izpolnjujete te zahteve:

- Windows 10 napravi je nameščena gradnja x64 1809 ali novejša različica.
- Nameščen je odjemalec za preprečevanje zlonamerne programske opreme, različica 4.18.2009.7 ali novejša.
- Naprava je **ena od** teh:
    
    - Azure Active Directory (Azure AD)
    - Hibridna storitev Azure AD, pridružena
    - Registriran AAD

- Če želite uveljaviti dejanja pravilnika, se prepričajte, Chromium v napravo s končno točko nameščen brskalnik Microsoft Chromium Edge.

Če želite dodatne zahteve za uvajanje preprečitve izgube končnih točk, glejte Uvod v [preprečitev izgube podatkov končne točke.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)