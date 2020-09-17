---
title: Napaka pri pošiljanju e-pošte, ki jo je blokiral SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783819"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Napaka pri pošiljanju e-pošte: gostitelj odjemalca je blokiran s storitvijo Spamhaus

Naslov IP, ki je poslal sporočilo, je na seznamu blokov, ki je v lasti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlogi za blokiranje s Spamhaus vključujejo ogrožene račune, ogrožene stroje, ki imajo v skupni rabi javni naslov IP in pravilnike internetnih storitev (ISP). Možni popravki so:
  
- Za blokirana dohodna sporočila, kjer nadzorujete izvorni e-poštni strežnik, morate določiti vzrok in odstraniti blok s spletnega mesta Spamhaus.

- Za blokirana dohodna sporočila, v katerih izvorni naslov IP pripada drugi osebi, mora lastnik naslova odstraniti blok s spletnega mesta Spamhaus. Če je naslov IP na seznamu za pravilnike (PBL), lahko lastnik dodeli drug statični naslov IP ali pa odstrani naslov iz PBL.

- Za blokirana odhodna sporočila iz domene, ki je povezana z Microsoftom, se lahko prikaže to sporočilo o napaki, če so sporočila preusmerjena v storitev tretje osebe. Z orodjem za iskanje v storitvi WHOIS lahko poiščete lastnika blokiranega naslova IP.
