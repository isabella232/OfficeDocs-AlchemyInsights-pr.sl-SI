---
title: orodje za izvoz e-odkrivanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 6352603a391ddcb44d2728c7587bf15a6cd97ebb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507186"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Ne morete namestiti ali zagnati orodja za izvoz e-odkrivanja?

Če ne morete namestiti ali zagnati orodja za izvoz e-odkrivanja za prenos rezultatov iskanja, preverite te stvari:
  
- Računalnik, ki ga uporabljate, izpolnjuje te predpogoje:

  - 32-ali 64-bitne različice operacijskega sistema Windows 7 in novejše različice

  - Microsoft .NET Framework 4,7

  - Podprt brskalnik:

  - Microsoft Edge

    Ali

  - Internet Explorer 10 in novejše različice

    Drugi brskalniki, kot sta Google Chrome in Mozilla Firefox, niso podprti.

- Vaša organizacija se lahko poveže s končno točko v storitvi Azure, ki je ** \* . blob.Core.Windows.net** (nadomestni znak predstavlja Enolični identifikator za vaše izvozno opravilo).

- Vlogo Export ste dodelili v središče za skladnost varnostnega središča Microsoft 365 &amp; . Ta vloga je privzeto dodeljena skupini vlog upravitelja e-odkrivanja. Glejte [dodeljevanje dovoljenj za e-odkrivanje](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Če želite več informacij, glejte [izvoz rezultatov iskanja po vsebini](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).
  