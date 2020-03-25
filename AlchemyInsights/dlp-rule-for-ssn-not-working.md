---
title: Pravilo DLP za SSN ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932551"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Težave DLP s številkami socialnega zavarovanja

**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju. Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve. V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.

V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi. Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih. Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.

**DLP težave s SSNs**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko socialnega zavarovanja (SSN)** pri uporabi občutljive vrste podatkov v Officeu 365? Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP. 
  
Na primer, za pravilnik SSN, konfiguriran z ravnjo zaupanja 85%, se ocenijo in morajo biti zaznani za pravilo, ki sproži:
  
- **[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 števk, ki so lahko v formatiranem ali neoblikovanem vzorcu

- **[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije iščejo SSNs v štirih različnih vzorcih:

  - Func_ssn najde SSNs s pre-2011 močno formatiranje, ki so oblikovane s črtice ali presledkov (DDD-DD-dddd ali DDD DD dddd)

  - Func_unformatted_ssn najde SSNs s pre-2011 močno oblikovanje, ki so neoblikovane kot devet zaporednih števk (ddddddddd)

  - Func_randomized_formatted_ssn najde post-2011 SSNs, ki so oblikovani s črtice ali presledkov (DDD-DD-dddd ali DDD DD dddd)

  - Func_randomized_unformatted_ssn najde post-2011 SSNs, ki so neoblikovane kot devet zaporednih števk (ddddddddd)

- **[Kontrolna vsota:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Ne, ni checksum

- **[Definicijo:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:

  - [Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) poišče vsebino, ki se ujema z vzorcem.

  - Najdena je ključna beseda iz [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Primeri ključnih besed vključujejo: *socialna varnost, socialna varnost #, SOC SEC, SSN* . Naslednji vzorec bi na primer sprožil pravilnik SSN za DLP: **SSN: 489-36-8350**
  
Če želite več informacij o tem, kaj je potrebno za iskanje SSN-ja za vašo vsebino, glejte naslednji razdelek v tem članku: [kaj vrste občutljivih informacij iščejo SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  