---
title: Pravilo OLP za SSN ne deluje
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004998"
---
# <a name="dlp-issues-with-social-security-numbers"></a>Težave s pravilnikom o DLP-jih s številkami socialnega zavarovanja

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave slp-jem s SSN-ji**

Ali imate težave s funkcijo za preprečevanje izgube podatkov **(DLP),** ki ne deluje za vsebino, ki vsebuje številko socialnega zavarovanja **(SSN),** če uporabljate občutljivo vrsto podatkov v Microsoft 365? V tem primeru se prepričajte, da vaša vsebina vsebuje potrebne informacije za iskanje pravilnika o dlpcih. 
  
Za pravilnik za SSN, konfiguriran z ravnijo zaupanja 85 %, se ovrednotijo in morajo biti zaznane, da se pravilo sproži:
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 števk, ki so lahko v oblikovanem ali neoblikovanih vzorcih

- **[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije poiščite SSN-je v štirih različnih vzorcih:

  - Func_ssn najde številke SSN, ki imajo pred leto 2011 močno oblikovanje, oblikovano s pomišljaji ali presledki (ddd-dd-dddd OR ddd dd dddd)

  - Func_unformatted_ssn najde številke SSN, ki so oblikovane pred letu 2011 in so oblikovane kot devet zaporednih številk (dddddddddd)

  - Func_randomized_formatted_ssn najde številke SSN, oblikovane s pomišljaji ali presledki po letu 2011 (ddd-dd-dddd OR ddd dd dddd);

  - Func_randomized_unformatted_ssn številke SSN po letu 2011, ki niso oblikovane in so devet zaporednih števk (dddddddddd)

- **[Kontrolna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, potrditvena vsota ni na voljo

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Pravilnik o DLP je 85 % prepričan, da je zaznal to vrsto občutljivih informacij, če znotraj bližine 300 znakov:

  - Funkcija [Func_ssn vsebino,](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) ki se ujema z vzorcem.

  - Najde se ključna [beseda Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) iz tega mesta. Primeri ključnih besed:  *Social Security, Social Security#, Soc Sec ,SSN*  . Ta vzorec bi sprožil pravilnik OSN za DLP: **SSN: 489-36-8350**
  
Če želite več informacij o tem, kaj je zahtevano, da so omrežja SSN zaznana za vašo vsebino, glejte ta razdelek v tem članku: Kaj vrste občutljivih informacij poiščite za [SSN-je](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Informacije o tem, kaj je zahtevano za druge vrste, najdete v tem članku: Kaj so vrste [občutljivih informacij?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  