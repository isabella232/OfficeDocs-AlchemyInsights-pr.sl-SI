---
title: DLP pravilo za številko kreditne kartice ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932459"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Težave z DLP s številkami kreditnih kartic

**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju. Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve. V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.

V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi. Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih. Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.

**Težave z DLP s številkami kreditnih kartic**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko kreditne kartice** pri uporabi vrste občutljivih informacij DLP v O365? Če je tako, preverite, ali vsebina vsebuje potrebne informacije, da sproži pravilnik DLP, ko je ovrednoten. Na primer, za **pravilnik o kreditni kartici** , konfigurirani z ravnjo zaupanja 85%, so ovrednotene naslednje in morajo biti odkrite za pravilo, ki sproži:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 številk, ki jih je mogoče formatirati ali neoblikovano (dddddddddddddddd) in mora opraviti test Luhn.

- **[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Zelo zapleten in robusten vzorec, ki zazna kartice iz vseh večjih blagovnih znamk po vsem svetu, vključno z Visa, MasterCard, Odkrijte Card, JCB, American Express, darilne kartice, in Diner kartice.

- **[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Da, Luhn ček

- **[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:

  - Funkcija Func_credit_card poišče vsebino, ki se ujema z vzorcem.

  - Nekaj od tega je res:

  - Najdena je ključna beseda iz Keyword_cc_verification.

  - Na voljo je ključna beseda iz Keyword_cc_name

  - Funkcija Func_expiration_date najde datum v pravem datumski obliki.

  - Kontrolna vsota prehaja

    Naslednji vzorec bi na primer sprožil pravilnik o številki kreditne kartice DLP:

  - Visa: 4485 3647 3952 7352
  
  - Poteče: 2/2009

Če želite več informacij o tem, kaj se zahteva za **številko kreditne kartice** , ki jo želite odkriti za vašo vsebino, glejte naslednji razdelek v tem članku: [katere vrste občutljivih informacij so na voljo za kreditno kartico #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  