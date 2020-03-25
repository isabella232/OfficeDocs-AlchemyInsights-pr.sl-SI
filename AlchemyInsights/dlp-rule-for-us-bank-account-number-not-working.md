---
title: Pravilo DLP za številko bančnega računa ZDA ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932566"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP težave z ameriški bančnega računa številke

**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju. Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve. V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.

V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi. Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih. Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.

**DLP težave z ameriški bančnega računa številke**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko bančnega računa ZDA** pri uporabi vrste občutljivih informacij DLP v O365? Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP, ko je ovrednoten.
  
Na primer, za pravilnik o **številki ameriškega bančnega računa** , ki je konfiguriran z ravnjo zaupanja 85%, se ocenijo naslednje in morajo biti odkrite za pravilo, ki sproži:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 števk

- **[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 zaporednih števk.

- **[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni checksum

- **[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:

  - Regularni izraz Regex_usa_bank_account_number najde vsebino, ki se ujema z vzorcem

  - Najdena je ključna beseda iz Keyword_usa_Bank_Account.

    Naslednji vzorec bi na primer sprožil pravilnik o **številki bančnega računa ZDA** : preverjanje računa 78344011

Če želite več informacij o tem, kaj je potrebno za iskanje **številke ameriškega bančnega računa** za vašo vsebino, glejte naslednji razdelek v tem članku: [katere vrste občutljivih informacij so na voljo za ŠTEVILKO bančnega računa ZDA](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  