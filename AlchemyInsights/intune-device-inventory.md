---
title: InTune inventarja naprave
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
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667894"
---
# <a name="intune-device-inventory"></a>InTune inventarja naprave

Rezilo» Devices «omogoča skrbniku vpogled v naprave v razdelku upravljanje v programu InTune v napravi na osnovi. Prikazani podatki vključujejo: strojna oprema, odkrite aplikacije, stanje naprave za skladnost s predpisi in stanje konfiguracije naprave.

Podatki o inventarju strojne opreme in odkriti programi so zbrani v sedemdnevnem ciklu. Aplikacije in določeni elementi strojne opreme se razlikujejo glede na operacijski sistem naprave in ali je naprava osebno ali v lasti podjetja.

Če želite več informacij, glejte [Ogled podrobnosti naprave v programu InTune](https://docs.microsoft.com/intune/device-inventory).

**Pogosta vprašanja**

V: v napravah s sistemom Windows ne prejmem celotnega seznama inventarnih programov, ki so na voljo v razdelku InTune. zakaj pa ne?

A: trenutno so v računalnikih s sistemom Windows 10, ki so prepoznani kot podjetja, navedene le sodobne aplikacije. InTune ne zbira informacij o aplikacijah Win32, ki so nameščene v teh napravah.

V: zakaj se telefonske številke ne zbirajo v vseh napravah?

A: telefoni, kategorizirani kot podjetja v programu InTune, niso identificirani s polno telefonsko številko, ko na primer zaženete poročilo o inventarju prenosne naprave. Telefonske številke, ki so na voljo za lastno napravo, so vedno delno prikrite z zvezdicami (* * * *) in prikazujejo le zadnje štiri števke.