---
title: 1491-Search-not-Returning-expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355893"
---
# <a name="content-search-not-returning-expected-results"></a>Vsebino iskanje ne vrne pričakovanih rezultatov

Ko teče vsebine iskanja iz Office 365 varnostno & Center skladnosti, se lahko prikaže nepričakovano zadetkov. Razmislite o naslednjih stvari, ki lahko vplivajo na rezultate iskanja:

- **Vsebine mesta in iskalne pogoje**: poskrbite, da boste izbrali ustrezno vsebine mesta in iskalne pogoje. Če ste zagnali veliko iskanje (z veliko lokacij), menijo, da razdelite v več iskanj.

- **Delno indeksirane postavke**: [delno indeksirane postavke](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) iz nabiralnikov so vključeni v rezultatih ocenjena. Vendar, delno indeksiranih elementi iz mesta in SharePoint OneDrive niso vključeni v oceni Išči.

- **Iskanje napak**: pri iskanju veliko število nabiralnikov (več kot 100.000 nabiralnikov), lahko dobite iskanje napak, s zmota zbornik CS008-009 in CS012-002). V tem primeru ponovite iskanje le ni vsebine mesta. Glej [Ta članek](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) za več informacij.
