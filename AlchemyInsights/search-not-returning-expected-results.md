---
title: 1491 – iskanje – ne – vračanje – pričakovano – rezultati
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740490"
---
# <a name="content-search-not-returning-expected-results"></a>Iskanje po vsebini ne vrne pričakovanih rezultatov

Ko zaženete iskanje vsebine iz središča za preverjanje varnosti & za skladnost s predpisi Microsoft 365, lahko prejmete nepričakovane rezultate iskanja. Razmislite o teh stvareh, ki lahko vplivajo na rezultate iskanja:

- **Mesta vsebine in pogoji iskanja**: Preverite, ali ste izbrali ustrezna mesta vsebine in pogoje iskanja. Če ste izvedli veliko iskanje (s številnimi lokacijami), jo razdelite na več iskanj.

- **Delno indeksirani elementi**:  [delno indeksirani elementi](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz nabiralnikov so vključeni v ocenjene rezultate iskanja. Vendar pa delno indeksirane elemente iz mest v SharePointu in OneDrive niso vključene v oceno iskanja.

- **Napake pri iskanju**: pri iskanju velikega števila nabiralnikov (prek 100.000 nabiralnikov) lahko pride do napak pri iskanju, s kodami napak, kot so CS008-009 in CS012-002). V tem primeru poskusite znova poiskati le neuspela mesta vsebine. Če želite več informacij, si oglejte  [Ta članek](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
