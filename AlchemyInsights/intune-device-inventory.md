---
title: Intune – inventar naprav
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014088"
---
# <a name="intune-device-inventory"></a>Intune – inventar naprav

Re blade Devices provides the administrator insight into devices under management in Intune on a per device basis. Prikazane informacije vključujejo: strojno opremo, odkrite aplikacije, stanje skladnosti naprave in stanje konfiguracije naprave.

Podatki o zalogi za strojno opremo in odkrite aplikacije se zbirajo v sedemdnevnem ciklu. Aplikacije in določeni elementi strojne opreme, o katerih je poročano, se razlikujejo glede na operacijski sistem naprave in glede na to, ali je naprava v lasti osebne naprave ali podjetja.

Če želite več informacij, glejte [Podrobnosti naprave v intune.](https://docs.microsoft.com/intune/device-inventory)

**Pogosta vprašanja**

V: Nisem prejel polnega seznama inventarja aplikacij, ki so na voljo v napravah, včlanjenih Windows Intune. zakaj pa ne?

O: Trenutno so za računalnike s sistemom Windows, Windows 10 navedene kot naprave podjetja, navedene le sodobne aplikacije. Intune ne zbira informacij o aplikacijah Win32, nameščenih v teh napravah.

V: Zakaj telefonske številke niso zbrane iz vseh naprav?

O: Telefoni, kategorizirani kot poslovne naprave v intune, niso prepoznani s polno telefonsko številko, če na primer zaženete poročilo o zalogi mobilne naprave. Telefonske številke iz naprave Bring-you-own-device so vedno delno zakrite z zvezdicami (****), in pokažejo le zadnje štiri števke.