---
title: Uporaba e-poštnih profilov s funkcijo InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653304"
---
# <a name="using-email-profiles-with-intune"></a>Uporaba e-poštnih profilov s funkcijo InTune

InTune lahko uporabite za ustvarjanje in uvajanje e-poštnih profilov za native (vgrajen) e-poštni odjemalec na več platformah naprav.

Če želite več informacij o nekaterih omejitvah, povezanih z e-poštnimi profili, vključno s tem, kako ravnati s prisotnostjo obstoječih profilov in kako odstraniti e-poštne profile, glejte [Dodajanje nastavitev e-pošte v naprave s funkcijo InTune](https://docs.microsoft.com/intune/email-settings-configure).

Če želite več informacij o tem, kako ustvarite profile e-pošte za vsako platformo naprave, glejte:

[Nastavitve naprave s sistemom Android za konfiguriranje e-pošte, preverjanja pristnosti in sinhronizacije v programu InTune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodajanje nastavitev e-pošte za naprave s sistemom iOS in iPadOS v programu Microsoft InTune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavitve e-poštnega profila v Microsoft InTune za naprave s sistemom Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavitve e-poštnega profila za naprave s sistemom Windows 10 v programu Microsoft InTune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Pogosta težava pri sinhronizaciji**

**KNOX v e-poštnem profilu s sistemom Android preprečuje, da bi bile uporabniške stike, koledar in opravila sinhronizirane z uporabniškimi napravami.**

V oknu KNOX v telefonu s sistemom Android KNOX se lahko odločite, katere vrste vsebine bodo sinhronizirane z napravo, in sicer tako, da nastavite vsako možnost.

Če je nastavitev za katero koli vrsto vsebine nastavljena na **ni konfigurirana** (privzeta), ta vrsta vsebine ni samodejno sinhronizirana. Uporabnik lahko želeno vrsto vsebine omogoči neposredno v napravi ročno, vendar je ta konfiguracija prepisana s nastavitev pravilnika InTune, sinhronizacije pa se ustavi za to vrsto vsebine.

