---
title: Pravilo DLP za SSN ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 5af843c2b70b5b2e1aaf82c9f01356546929d840
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43788718"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Težave DLP s številkami socialnega zavarovanja

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP težave s SSNs**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko socialnega zavarovanja (SSN)** pri uporabi občutljive vrste podatkov v Microsoft 365? Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP. 
  
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
  