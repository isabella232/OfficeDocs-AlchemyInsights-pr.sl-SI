---
title: 1491-search-not-returning-expected-results
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
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052726"
---
# <a name="content-search-not-returning-expected-results"></a>Iskanje vsebine ne vrača pričakovanih rezultatov

Pri zagonu iskanja po vsebini iz središča Microsoft 365 za & za skladnost s predpisi lahko prejmete nepričakovane rezultate iskanja. Razmislite o tem, kaj lahko vpliva na rezultate iskanja:

- **Mesta vsebine in pogoji iskanja**: Preverite, ali ste izbrali ustrezna mesta vsebine in pogoje iskanja. Če ste zagnali veliko iskanje (z veliko lokacijami), ga razdelite na več iskanih mest.

- **Delno indeksirani elementi:**  [Delno indeksirani elementi iz](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) nabiralnikov so vključeni v ocenjene rezultate iskanja. Delno indeksirani elementi z mest v SharePoint in OneDrive niso vključeni v oceno iskanja.

- Napake **pri** iskanju: Pri iskanju velikega števila nabiralnikov (več kot 100.000 nabiralnikov) lahko pride do napak pri iskanju s kodami napak, kot sta CS008-009 in CS012-002). V tem primeru poskusite znova poiskati le mesta neuspele vsebine. Več  [informacij najdete v](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) tem članku.
