---
title: orodje za izvoz e-odkrivanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36736341"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Ne morete namestiti ali zagnati orodja za izvoz e-odkrivanja?

Če ne morete namestiti ali zagnati sistema Office 365 eDiscovery Export Tool za prenos rezultatov iskanja, preverite naslednje stvari:
  
- Računalnik, ki ga uporabljate, izpolnjuje te predpogoje:

  - 32-ali 64-bitne različice operacijskega sistema Windows 7 in novejše različice

  - Microsoft .NET Framework 4,7

  - Podprt brskalnik:

  - Microsoft Edge

    Ali

  - Internet Explorer 10 in novejše različice

    Drugi brskalniki, kot sta Google Chrome in Mozilla Firefox, niso podprti.

- Vaša organizacija se lahko poveže s končno točko v storitvi Azure, ki je ** \*. blob.Core.Windows.net** (nadomestni znak predstavlja Enolični identifikator za vaše izvozno opravilo).

- Vlogo Export ste dodelili v središče za skladnost varnostnega &amp; sistema Office 365. Ta vloga je privzeto dodeljena skupini vlog upravitelja e-odkrivanja. Glejte [dodeljevanje dovoljenj za e-odkrivanje](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions).

Če želite več informacij, glejte [izvoz rezultatov iskanja po vsebini](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  