---
title: Inventar naprave Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440477"
---
# <a name="intune-device-inventory"></a>Inventar naprave Intune

Rezilo Naprave omogoča skrbniku vpogled v naprave, ki jih upravljali v intunu, na podlagi naprave. Prikazane informacije vključujejo: Strojna oprema, Odkrite aplikacije, Stanje skladnosti naprave in stanje konfiguracije naprave.

Podatki o zalogah za strojno opremo in odkrite aplikacije se zbirajo v sedemdnevnem ciklu. Aplikacije in posebni elementi strojne opreme, o katerih so poročali, se razlikujejo glede na operacijski sistem naprave in ali je naprava v zasebni lasti ali v lasti podjetja.

Če želite več informacij, [glejte Ogled podrobnosti o napravi v intune](https://docs.microsoft.com/intune/device-inventory).

**Pogosta vprašanja**

V: Ne prejemam celotnega seznama inventarja aplikacij, ki so prisotne v napravah Windows, vpisanih v Intune. zakaj pa ne?

O: Trenutno so za računalnike s sistemom Windows 10, ki so prepoznani kot poslovne naprave, navedene samo sodobne aplikacije. Intune ne zbira podatkov o aplikacijah Win32, nameščenih v teh napravah.

V: Zakaj telefonske številke niso zbrane iz vseh naprav?

O: Telefoni, ki so v intunu razvrščeni kot poslovne naprave, niso identificirani s polno telefonsko številko, ko na primer zaženete poročilo o inventarju mobilne naprave. Številke telefonov Bring-you-own-device so vedno delno zakrite z zvezdicami (****) in prikazujejo samo zadnje štiri števke.