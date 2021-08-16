---
title: Pravilo OLP za ZDA/Združeno kraljestvo – številka potnega lista ne deluje
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004962"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Težave s DLP-jem – številka potnega lista v ZDA/Združenem kraljestvu

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave s DLP-jem s številkami potnega lista v ZDA/Združenem kraljestvu**

Ali imate težave s preprečitev izgube **podatkov,** ki ne deluje za vsebino, ki vsebuje številko potnega lista v **ZDA/Združenem** kraljestvu, ko uporabljate vrsto občutljivih podatkov za preprečitev izgube podatkov v storitvi O365? V tem primeru se prepričajte, da vsebina vsebuje potrebne informacije za to, kar išče pravilnik o DLP, ko se ovrednoti.
  
Na primer, za pravilnik o številki potnega lista v **ZDA/Združenem** kraljestvu, konfiguriran z stopnjo zaupanja 75 %, se to ovrednoti in mora biti zaznano, da pravilo sproži
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet števk

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet zaporednih števk

- **[Kontrolna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, potrditvena vsota ni na voljo

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Pravilnik o DLP je 75 % prepričan, da je zaznal to vrsto občutljivih informacij, če znotraj bližine 300 znakov:

  - Funkcija Func_usa_uk_passport najde vsebino, ki se ujema z vzorcem.

  - Najde se ključna beseda Keyword_passport iz tega mesta.

    Na primer, ta vzorec bi sprožil pravilnik za številko potnega lista v **ZDA/Združenem** kraljestvu: ZDA Številka potnega 123456789

Če želite več informacij o zahtevah, da je za vašo vsebino zaznana številka potnega lista za ZDA/Združeno kraljestvo, si oglejte ta razdelek v tem članku: Kakšna je vrsta občutljivih informacij za [ZDA/Združeno](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) kraljestvo Passport Number
  
Informacije o tem, kaj je zahtevano za druge vrste, najdete v tem članku: Kaj so vrste [občutljivih informacij?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  