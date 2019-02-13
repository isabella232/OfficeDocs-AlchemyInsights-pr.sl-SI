---
title: Napaka, pošiljanje e-pošte, ki blokira SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912364"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Napaka pri pošiljanju e-pošte: odjemalca gostitelja blokiran z Spamhaus

IP naslov, ki je poslal sporočilo, je na seznamu blokiranih mest v lasti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlogi za blokirala Spamhaus vključujejo ogrožena računov, ogrožena stroji delitev javni IP naslov in ponudnika internetnih storitev (ISP) pravila. Možni popravki so:
  
- Za blokirane dohodna sporočila Office 365, če nadzirate strežnik vir e-pošte, boste morali ugotoviti vzrok in odstrani blokiranja na spletni strani Spamhaus.
    
- Za blokirane dohodna sporočila Office 365, kjer izvorni IP naslov pripada nekomu drugemu, naslov lastnik mora umakniti blok na spletni strani Spamhaus. Če je IP naslov na seznam blok politike (PBL), lastnik lahko dodelite različne statični naslov IP ali naslov odstranite na PBL.
    
- Za blokirane odhodnih sporočil iz vaše domene Office 365, lahko prejmete to napako, če sporočila so preusmerjeni preko 3rd stranka storitev. Uporabite lahko orodje za iskanje WHOIS najti lastnika blokiranih IP naslov.
    

