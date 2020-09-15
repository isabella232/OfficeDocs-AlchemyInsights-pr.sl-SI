---
title: Pravilo DLP za SSN ne deluje
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679385"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Težave z DLP s številkami socialnega zavarovanja

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave z DLP s številke SSN**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** ne delate za vsebino, ki vsebuje **številko socialnega zavarovanja (SSN)** , ko uporabljate občutljivo vrsto podatkov v programu Microsoft 365? Če je tako, se prepričajte, da vaša vsebina vsebuje potrebne informacije o tem, kaj išče pravilnik DLP. 
  
Na primer za pravilnik SSN, konfiguriran z ravnjo zaupanja 85%, se ocenijo in jih je treba zaznati, da bo pravilo sprožilo:
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 številk, ki so lahko v oblikovanem ali neoblikovanem vzorcu

- **[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije poiščite številke SSN v štirih različnih vzorcih:

  - Func_ssn najde številke SSN z močnim oblikovanjem vnaprej 2011, ki so oblikovani s pomišljaji ali presledki (DDD-DD-dddd ali DDD DD dddd)

  - Func_unformatted_ssn najde številke SSN z močnim oblikovanjem vnaprej 2011, ki niso oblikovani kot devet zaporednih števk (ddddddddd)

  - Func_randomized_formatted_ssn najde številke SSN za 2011, ki so oblikovani s pomišljaji ali presledki (DDD-DD-dddd ali DDD DD dddd)

  - Func_randomized_unformatted_ssn najde 2011 številke SSN, ki niso oblikovani kot devet zaporednih števk (ddddddddd)

- **[Preskusna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, ni checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če je v bližini 300 znakov:

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) najde vsebino, ki se ujema z vzorcem.

  - Najde se ključna beseda iz [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Primeri ključnih besed vključujejo:  *socialno varnost, socialno varnost #, SOC SEC, SSN*  . Naslednji vzorec bi na primer sprožil pravilnik DLP: **SSN: 489-36-8350**
  
Če želite več informacij o tem, kaj je potrebno za odkrivanje številke SSN za vašo vsebino, si oglejte ta razdelek v tem članku: [Kaj so občutljive vrste informacij za številke SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Če uporabljate drugačno vgrajeno občutljivo vrsto informacij, si oglejte ta članek za informacije o tem, kaj je zahtevano za druge vrste: [Kaj so videti občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  