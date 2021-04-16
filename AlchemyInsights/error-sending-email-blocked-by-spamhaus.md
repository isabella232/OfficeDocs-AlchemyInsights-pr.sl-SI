---
title: Napaka pri pošiljanju e-pošte, ki jo blokira SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813740"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Napaka pri pošiljanju e-pošte: Spamhaus blokira odjemalca gostitelja

Naslov IP, s katerega je bilo poslano sporočilo, je na seznamu blokiranih naslovov, ki je v [lasti podjetja Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Med razloge za blokiranje s strani podjetja Spamhaus spadajo ogroženi računi, ogroženi računalniki, ki delijo javni naslov IP, in pravilniki ponudnikov internetnih storitev (ISP). Možne popravke so:
  
- Za blokirana dohodna sporočila, kjer nadzirate izvorni e-poštni strežnik, morate določiti vzrok in odstraniti blokado s spletnega mesta Spamhaus.

- Za blokirana dohodna sporočila, kjer naslov IP pripada nekomu drugemu, mora lastnik naslova odstraniti blokado s spletnega mesta Spamhaus. Če je naslov IP na seznamu blokiranih pravilnikov (PBL), lahko lastnik dodeli drugačen statični naslov IP ali odstrani naslov s seznama PBL.

- Za blokirana odhodna sporočila iz vaše domene, povezane z Microsoftom, lahko to sporočilo o napaki prejmete, če so sporočila usmerjanje prek storitve drugega ponudnika. Z orodjem za iskanje WHOIS lahko najdete lastnika blokiranega naslova IP.
