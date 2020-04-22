---
title: AntiSpam 5.4.1 DBEB Catch-vse
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707927"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Fix dostava vprašanja za kodo napake 550 5.4.1 Relay dostop zavrnjen

Do te težave pride, ko [preverjate, ali je e-poštni naslov veljaven za preprečitev odskakanja](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ob vstopu v Microsoftovo omrežje. Poskusite naslednje:

1. Ugotovite, ali je težava specifična za celotno domeno ali en sam e-poštni naslov:
    - Celotna domena: včasih domeno je treba sinhronizirati; začeti [postavljanje področje v notranji ter torej prislon v verodostojni](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - En e-poštni naslov: včasih je treba naslov sinhronizirati; Spreminjanje naslova strežnika SMTP in ga nato spremeni nazaj, lahko pomaga.
2. Ugotovite, ali je težava specifična za skupino ali javno mapo. Za nekatere vrste predmetov bo morda treba predmete ročno ustvariti v storitvi Azure Active Directory.

Če potrebujete dodatno pomoč, odprite vstopnico za podporo in določite obseg težave (vključno z vrsto predmeta, ki ga pošiljate), da vam lahko pomagamo bolje.