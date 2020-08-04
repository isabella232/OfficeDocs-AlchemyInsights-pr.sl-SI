---
title: Uporaba e-poštnih profilov s storitvijo Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555761"
---
# <a name="using-email-profiles-with-intune"></a>Uporaba e-poštnih profilov s storitvijo Intune

Intune se lahko uporablja za ustvarjanje in uvajanje e-poštnih profilov za izvornega (vgrajenega) e-poštnega odjemalca na več platformah naprav.

Če želite več informacij o nekaterih omejitvah, povezanih z e-poštnimi profili, vključno s tem, kako se obravnava prisotnost obstoječih profilov in kako [odstraniti e-poštne profile, glejte Dodajanje e-poštnih nastavitev napravam s storitvijo Intune](https://docs.microsoft.com/intune/email-settings-configure).

Če želite več informacij o ustvarjanju e-poštnih profilov za vsako platformo naprave, glejte:

[Nastavitve naprave Android za konfiguracijo e-pošte, preverjanja pristnosti in sinhronizacije v intunu](https://docs.microsoft.com/intune/email-settings-android)  
[Dodajanje nastavitev e-pošte za naprave s sistemom iOS in iPadOS v storitvi Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Nastavitve e-poštnega profila v storitvi Microsoft Intune za naprave s sistemom Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Nastavitve e-poštnega profila za naprave s sistemom Windows 10 v storitvi Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Pogosta težava pri sinhronizaciji**

**Knox v e-poštnem profilu za Android preprečuje sinhronizacijo uporabniških stikov, koledarja in opravil z uporabniškimi napravami.**

Knox na Android Knox e-poštni profil ponuja admin možnost, da se odločijo, katere vrste vsebine so sync'd z napravo z nastavitvijo vsak omogočen.

Če je nastavitev za katero koli od vrst vsebine **nastavljena na Ni konfigurirano** (privzeto), se ta vrsta vsebine ne sinhronizira samodejno. Uporabnik lahko omogoči vrsto vsebine, ki jo želijo, neposredno v napravi ročno, vendar je ta konfiguracija prepisana z nastavitvijo pravilnika Intune, sinhronizacija pa se ustavi za to vrsto vsebine.

