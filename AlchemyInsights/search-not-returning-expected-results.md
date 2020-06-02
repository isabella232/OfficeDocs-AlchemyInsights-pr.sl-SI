---
title: 1491-iskanje-ne vrača-pričakovani-rezultati
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510588"
---
# <a name="content-search-not-returning-expected-results"></a>Iskanje vsebine ne vrača pričakovanih rezultatov

Ko izvajate iskanja po vsebini iz Microsoft 365 Security & center za skladnost, lahko prejmete nepričakovane rezultate iskanja. Razmislite o naslednjih stvareh, ki lahko vplivajo na rezultate iskanja:

- **Mesta vsebine in pogoji iskanja**: Prepričajte se, da ste izbrali ustrezne lokacije vsebine in iskalne pogoje. Če ste zagnali veliko iskanje (z mnogimi lokacijami), razmislite o razdelitvi v več iskanj.

- **Delno indeksirani elementi**: [delno indeksirani elementi](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz nabiralnikov so vključeni v ocenjene rezultate iskanja. Vendar pa delno indeksirani elementi iz mest v SharePointu in storitvi OneDrive niso vključeni v oceno iskanja.

- **Napake pri iskanju**: pri iskanju velikega števila nabiralnikov (več kot 100.000 nabiralnikov) lahko dobite napake pri iskanju, s kodami napak, kot sta CS008-009 in CS012-002). V tem primeru poskusite znova iskati samo za neuspele lokacije vsebine. Za več informacij glejte [Ta članek](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
