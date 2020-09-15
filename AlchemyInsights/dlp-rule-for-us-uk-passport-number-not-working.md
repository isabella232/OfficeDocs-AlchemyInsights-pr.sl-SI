---
title: Pravilo DLP za številko potnega lista US/UK ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679240"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Težave s številkami potnega lista za DLP – US/UK

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave z DLP s številkami potnega lista ZDA/UK**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** ne delate za vsebino, ki vsebuje **številko potnega lista ZDA/UK** , ko uporabljate vrsto občutljivih podatkov DLP v O365? Če je tako, se prepričajte, da vaša vsebina vsebuje potrebne informacije o tem, kaj išče pravilnik DLP, ko ga ocenite.
  
Na primer, za pravilnik **številka potnega lista ZDA/UK** , konfiguriran z ravnjo zaupanja 75%, je treba ovrednotiti te in jih je treba zaznati, da bo pravilo sprožilo
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet števk

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet zaporednih števk

- **[Preskusna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ni checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če je v bližini 300 znakov:

  - Funkcija Func_usa_uk_passport najde vsebino, ki se ujema z vzorcem.

  - Najde se ključna beseda iz Keyword_passport.

    Na primer, naslednji vzorec bi sprožilo za pravilnik **številka potnega lista ZDA/UK** : us Passportova številka 123456789

Če želite več informacij o tem, kaj je potrebno za številko Passporta ZDA/UK, ki jo želite zaznati za vašo vsebino, si oglejte ta razdelek v tem članku: [Kaj so občutljive vrste informacij za US/UK številka potnega lista](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Če uporabljate drugačno vgrajeno občutljivo vrsto informacij, si oglejte ta članek za informacije o tem, kaj je zahtevano za druge vrste: [Kaj so videti občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  