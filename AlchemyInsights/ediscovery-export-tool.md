---
title: Orodje za izvoz e-odkrivanja
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101318"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Ali ne morete namestiti ali zagnati orodja za izvoz e-odkrivanja?

Če ne morete namestiti ali zagnati orodja za izvoz e-odkrivanja, da bi prenesli rezultate iskanja, preverite te elemente:
  
- Računalnik, ki ga uporabljate, izpolnjuje te zahteve:

  - 32- ali 64-bitne različice Windows 7 in novejše različice

  - Microsoft .NET Framework 4.7

  - Podprt brskalnik:

  - Microsoft Edge

    Ali

  - Internet Explorer 10 in novejše različice

    Drugi brskalniki, kot sta Google Chrome in Mozilla Firefox, niso podprti.

- Vaša organizacija se lahko poveže s končno točko v storitvi Azure, ki je **\* .blob.core.windows.net** (nadomestni znak predstavlja enolični identifikator za posel izvoza).

- Dodeljena vam je vloga za izvoz v središču za Microsoft 365 za &amp; skladnost s predpisi. Privzeto je ta vloga dodeljena le skupini vlog upravitelja e-odkrivanja. Glejte [Dodeljevanje dovoljenj za e-odkrivanje.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Če želite več informacij, glejte [Izvoz rezultatov iskanja po vsebini.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Če izvažate več kot 100.000 nabiralnikov, morate za prenos rezultatov izvoza uporabiti to storitev Powershell: Izvoz rezultatov iz več kot [100 K nabiralnikov.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)