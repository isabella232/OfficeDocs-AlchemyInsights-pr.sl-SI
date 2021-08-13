---
title: Uporaba e-poštnih profilov s storitvijo Intune
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
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919439"
---
# <a name="using-email-profiles-with-intune"></a>Uporaba e-poštnih profilov s storitvijo Intune

Intune lahko uporabite za ustvarjanje in uvajanje e-poštnih profilov za izvornega (vgrajenega) e-poštnega odjemalca v več platformah naprave.

Če želite informacije o nekaterih omejitvah, povezanih z e-poštnimi profili, vključno s tem, kako se obravnava prisotnost obstoječih profilov in kako odstranite e-poštne profile, glejte Dodajanje nastavitev e-pošte v naprave, ki uporabljajo [Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Če želite več informacij o ustvarjanju e-poštnih profilov za posamezno platformo naprave, glejte:

[Nastavitve naprave s sistemom Android za konfiguracijo e-pošte, preverjanja pristnosti in sinhronizacije v intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodajanje nastavitev e-pošte za naprave s sistemom iOS in iPadOS v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavitve e-poštnega profila v Microsoft Intune za naprave, v Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavitve e-poštnega profila za naprave s Windows 10 v Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Pogosta težava s sinhronizacijo**

**KnOX v e-poštnem profilu sistema Android preprečuje sinhronizacijo stikov, koledarja in opravil s uporabniškimi napravami.**

E-poštni profil KNOX v sistemu Android KNOX ponuja skrbniku možnost, da določi, katere vrste vsebine bodo sinhronizirane z napravo, tako da vsako možnost nastavite na omogočeno.

Če je nastavitev za katero koli vrsto vsebine nastavljena na Ni **konfigurirano** (privzeto), se ta vrsta vsebine ne sinhronizira samodejno. Uporabnik bo morda omogočil vrsto vsebine, ki jo želi neposredno v napravi, vendar bo nastavitev pravilnika za Intune prepisala konfiguracijo, sinhronizacija za to vrsto vsebine pa se ustavi.

