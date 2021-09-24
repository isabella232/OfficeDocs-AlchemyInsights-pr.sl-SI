---
title: Zamenjava Microsoftovih imenskih strežnikov z upravljanjem zapisov DNS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506973"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Zamenjava Microsoftovih imenskih strežnikov z upravljanjem zapisov DNS

Prej ste spremenili zapise imen strežnika, da kažejo na Microsoft (ns1.bdm.microsoftonline.com), vendar ste se odločili, da boste zdaj upravljali svoje zapise DNS:

Na spletnem mestu registratorja domene spremenite imenski strežnik nazaj na svojega registratorja ali prejšnjo nastavitev. Če ne poznate sistema DNS, se obrnite na podporo registratorja domene. Upoštevajte, da lahko traja do 48 ur, da se spremembe imenskega strežnika razširijo. 

1. V skrbniškem portalu Microsoft 365 pojdite na **Nastavitve** Domene , potrdite potrditveno polje ob domeni in  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)izberite Manage **DNS (Upravljanje zapisov DNS).** 

2. V čarovniku izberite **Dodajte svoje zapise DNS in** dokončajte čarovnika. S tem spremenite način upravljanja zapisov DNS, nato pa dodate zapise DNS po meri, ki jih potrebujete za podporo izbranih storitev.

Ali pa, če ste spremenili zapise imenskega strežnika na Microsoft in imate spletno mesto, lahko dodate zapise DNS za spletno mesto, namesto da bi spremenili imenske strežnike nazaj. Če želite več informacij, glejte [Posodobitev zapisov DNS za obdržite spletno mesto pri trenutnem ponudniku gostovanja.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


