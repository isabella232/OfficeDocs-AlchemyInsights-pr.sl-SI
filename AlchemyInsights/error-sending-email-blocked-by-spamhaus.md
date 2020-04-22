---
title: Napaka pri pošiljanju e-pošte blokirana, ki jih SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714274"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Napaka pri pošiljanju e-pošte: odjemalec gostitelja blokiran z Spamhaus

IP naslov, ki je poslal sporočilo, je na blok seznam v lasti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlogi za blokado s strani Spamhaus vključujejo ogrožene račune, ogrožene stroje, ki delijo javni naslov IP in pravilnike ponudnika internetnih storitev (ISP). Možni popravki so:
  
- Za blokirana dohodna sporočila, kjer nadzirate izvorni e-poštni strežnik, morate ugotoviti vzrok in odstraniti blok iz spletne strani Spamhaus.

- Za blokirana dohodna sporočila, kjer je izvorni IP naslov pripada nekomu drugemu, mora lastnik naslova odstraniti blok iz spletne strani Spamhaus. Če je naslov IP na seznamu blokiranih pravilnikov (PBL), lahko lastnik dodeli drug statični naslov IP ali odstrani naslov iz PBL.

- Za blokirana odhodna sporočila iz vaše domene, povezane z Microsoftom, lahko to napako prejmete, če so sporočila preusmerjena skozi storitev 3rd Party. Za iskanje blokiranega lastnika naslova IP lahko uporabite orodje za iskanje WHOIS.
