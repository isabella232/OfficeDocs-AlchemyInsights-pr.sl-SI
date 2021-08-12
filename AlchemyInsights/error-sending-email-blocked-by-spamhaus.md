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
ms.openlocfilehash: 8372032e19bd2ebaf3ba8cc8e87f19ef3e2edf1e607b1739a919f6dcc443cd97
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946787"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Napaka pri pošiljanju e-pošte: Spamhaus blokira odjemalca gostitelja

Naslov IP, s katerega je bilo poslano sporočilo, je na seznamu blokiranih naslovov, ki je v [lasti podjetja Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Med razloge za blokiranje s strani podjetja Spamhaus spadajo ogroženi računi, ogroženi računalniki, ki delijo javni naslov IP, in pravilniki ponudnikov internetnih storitev (ISP). Možne popravke so:
  
- Za blokirana dohodna sporočila, kjer nadzirate izvorni e-poštni strežnik, morate določiti vzrok in odstraniti blokado s spletnega mesta Spamhaus.

- Za blokirana dohodna sporočila, kjer naslov IP pripada nekomu drugemu, mora lastnik naslova odstraniti blokado s spletnega mesta Spamhaus. Če je naslov IP na seznamu blokiranih pravilnikov (PBL), lahko lastnik dodeli drugačen statični naslov IP ali odstrani naslov s seznama PBL.

- Za blokirana odhodna sporočila iz vaše domene, povezane z Microsoftom, lahko to sporočilo o napaki prejmete, če so sporočila usmerjanje prek storitve drugega ponudnika. Z orodjem za iskanje WHOIS lahko najdete lastnika blokiranega naslova IP.
