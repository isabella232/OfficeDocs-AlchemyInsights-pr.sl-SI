---
title: AntiSpam 5.4.1 DBEB Catch-All
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717377"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Odpravljanje težav z dostavo za kodo napake 550 za dostop do posredovanja

Do te težave pride pri [preverjanju, ali je e-poštni naslov veljaven, da preprečite bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pri vnosu Microsoftovega omrežja. Preskusite to:

1. Določite, ali je težava značilna za celotno domeno ali en e-poštni naslov:
    - Celotna domena: včasih je treba domeno sinhronizirati; poskusite [nastaviti domeno na notranjo in nato spet na avtoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - En e-poštni naslov: včasih je treba naslov sinhronizirati; Če želite spremeniti naslov strežnika proxy SMTP in ga nato znova spremeniti, lahko pomagate.
2. Določite, ali je težava značilna za skupino ali javno mapo. Za nekatere vrste predmetov morajo biti predmeti morda ročno ustvarjeni v storitvi Azure Active Directory.

Če potrebujete dodatno pomoč, odprite vstopnico za podporo in določite obseg težave (vključno z vrsto predmeta, ki ga pošiljate), tako da vam lahko pomagamo bolje.