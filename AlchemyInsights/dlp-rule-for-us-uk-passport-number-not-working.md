---
title: DLP pravilo za ZDA / UK številka potnega lista, ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529935"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Težave z DLP - ZDA / UK številke potnega lista

Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebine, ki vsebuje a **ZDA / UK številka potnega lista** čas using DLP tip zelo občutljliv sporočilo v O365? Če je tako, poskrbite, da vaša vsebina vsebuje potrebne informacije za kaj je politika DLP iščejo, ko je ovrednotena.
  
Na primer na **US / UK številka potnega lista** pravilnik, konfiguriran s 75 odstotno stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži
  
- **[Oblika:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet števk

- **[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet zaporednih številk

- **[Ček:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni ne ček

- **[Opredelitev:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika je 75 % prepričana, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov:

  - Vsebina, ki ustreza vzorcu ugotovi, funkcijo Func_usa_uk_passport.

  - Ključno besedo iz Keyword_passport je našel.

    Na primer, bi ta vzorec sproži za v **ZDA / UK številka potnega lista** politike: številka potnega lista ZDA 123456789

Za več informacij o tem, kaj je potrebno za ZDA / UK številka potnega lista z zazna za vašo vsebino, glejte razdelek naslednje v tem članku: [Kaj je občutljive vrste informacij iščejo ZDA / UK številka potnega lista](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  