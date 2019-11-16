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
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672449"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Fix dostava vprašanja za kodo napake 550 5.4.1 Relay dostop zavrnjen

Do te težave pride, ko [preverjate, ali je e-poštni naslov veljaven, da preprečite bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) ob vstopu v omrežje Office 365. Poskusite naslednje:

1. Ugotovite, ali je težava specifična za celotno domeno ali en sam e-poštni naslov:
    - Celotna domena: včasih domeno je treba sinhronizirati; začeti [postavljanje področje v notranji ter torej prislon v verodostojni](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - En e-poštni naslov: včasih je treba naslov sinhronizirati; Spreminjanje naslova strežnika SMTP in ga nato spremeni nazaj, lahko pomaga.
2. Ugotovite, ali je težava specifična za skupino ali javno mapo. Za nekatere vrste predmetov bo morda treba predmete ročno ustvariti v storitvi Azure Active Directory.

Če potrebujete dodatno pomoč, odprite vstopnico za podporo in določite obseg težave (includidng vrsto predmeta, ki ga pošiljate), da vam lahko pomagamo bolje.