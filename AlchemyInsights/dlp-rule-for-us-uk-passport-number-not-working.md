---
title: Pravilo DLP za številko potnega lista ZDA/UK ne deluje
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
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931278"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Težave s številkami potnih listov DLP-US/UK

**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju. Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve. V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.

V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi. Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih. Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.

**DLP vprašanja z ZDA/UK številke potnega lista**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko potnega lista ZDA/UK** pri uporabi vrste občutljivih informacij DLP v O365? Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP, ko je ovrednoten.
  
Na primer, za pravilnik o **številki potnega lista ZDA/UK** , konfigurirani z ravnjo zaupanja 75%, se ocenijo in morajo biti odkrite za pravilo, ki sproži
  
- **[Oblika zapisa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Devet števk

- **[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Devet zaporednih števk

- **[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni checksum

- **[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:

  - Funkcija Func_usa_uk_passport poišče vsebino, ki se ujema z vzorcem.

  - Najdena je ključna beseda iz Keyword_passport.

    Na primer, naslednji vzorec bi sprožila za **ZDA/UK številka potnega lista** politike: us passport številka 123456789

Za več informacij o tem, kaj je potrebno za ZDA/UK številka potnega lista, ki se zazna za vašo vsebino, glejte naslednji razdelek v tem članku: [Kaj občutljive vrste informacij IŠČEJO ZDA/UK Passport številka](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  