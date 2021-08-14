---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932293"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Odpravljanje težav z dostavo kode napake 550 5.4.1 zavrnjen dostop do posredovalnega strežnika

Do te težave pride pri preverjanju, ali je e-poštni naslov veljaven in preprečuje povratne podatke o [odklonih, ko](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) vnašate podatke v Microsoftovo omrežje. Poskusite to:

1. Določite, ali je težava specifična za celotno domeno ali en e-poštni naslov:
    - Celotna domena: včasih je treba domeno sinhronizirati; poskusite [nastaviti domeno na Notranje in nato nazaj na Avtoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - En e-poštni naslov: včasih je treba naslov sinhronizirati; lahko pomagate tako, da spremenite naslov proxy smtp in ga nato znova spremenite.
2. Določite, ali je težava specifična za skupino ali javno mapo. Za nekatere vrste predmetov boste morda morali predmete ustvariti ročno v Azure Active Directory.

Če potrebujete dodatno pomoč, odprite vstopnico za podporo in določite obseg težave (vključno z vrsto predmeta, na katere pošiljate), da vam bomo lahko pomagali bolje.