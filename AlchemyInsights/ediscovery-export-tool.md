---
title: orodje za izvoz E-odkrivanje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277944"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Ne morete namestiti ali zagnati orodja za izvoz E-odkrivanje?

Če ne morete namestiti ali zagnati orodja za izvoz E-odkrivanje za prenos rezultatov iskanja, si oglejte te stvari:
  
- Računalnik, ki ga uporabljate, izpolnjuje te pogoje:

  - 32-ali 64-bitne različice sistema Windows 7 in novejše različice

  - Microsoft .NET Framework 4.7

  - Podprt brskalnik:

  - Microsoft Edge

    Ali

  - Internet Explorer 10 in novejše različice

    Drugi brskalniki, kot sta Google Chrome in Mozilla Firefox, niso podprti.

- Vaša organizacija se lahko poveže s končno točko v storitvi Azure, ki je ** \* . blob.Core.Windows.net** (nadomestni znak predstavlja Enolični identifikator za izvozno opravilo).

- Izvozna vloga je dodeljena v središču za skladnost z varnostnim preverjanjem za Microsoft 365 &amp; . Ta vloga je privzeto dodeljena le skupini vlog E-odkrivanje Manager. Glejte [dodeljevanje dovoljenj za e-odkrivanje](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Če želite več informacij, glejte [izvoz rezultatov iskanja vsebine](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Če izvažate več kot 100K nabiralnike, boste morali uporabiti ta PowerShell za prenos rezultatov izvoza:  [izvažanje rezultatov iz več kot 100k nabiralnikov](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).