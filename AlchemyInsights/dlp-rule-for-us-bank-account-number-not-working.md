---
title: Pravilo o dlpciji za številko bančnega računa v ZDA ne deluje
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005034"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Težave s dlpcijo s številkami bančnih računov v ZDA

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave s dlpcijo s številkami bančnih računov v ZDA**

Ali imate težave s preprečevanjem izgube podatkov **(DLP)** ne deluje za vsebino, ki vsebuje številko bančnega računa v ZDA, ko uporabljate vrsto občutljivih podatkov za preprečitev izgube podatkov v storitvi O365?  V tem primeru se prepričajte, da vsebina vsebuje potrebne informacije za to, kar išče pravilnik o DLP, ko se ovrednoti.
  
Na primer, pri **pravilniku ZDA o** številki bančnega računa, konfiguriranem s stopnjo zaupanja 85 %, se ovrednotijo te nastavitve in jih je treba zaznati, da pravilo sproži:
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 števk

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 zaporednih števk.

- **[Kontrolna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, potrditvena vsota ni na voljo

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Pravilnik o DLP je 75 % prepričan, da je zaznal to vrsto občutljivih informacij, če znotraj bližine 300 znakov:

  - Regularni izraz, Regex_usa_bank_account_number najde vsebino, ki se ujema z vzorcem

  - Najde se ključna beseda Keyword_usa_Bank_Account iz te vrste.

    Ta primer bi sprožil pravilnik o številki bančnega računa v **ZDA:** Checking Account 78344011

Če želite več informacij o  zahtevah, da je za vašo vsebino zaznana številka bančnega računa v ZDA, si oglejte ta razdelek v tem članku: Kakšna je vrsta občutljivih informacij za ŠTEVILKO bančnega računa v [ZDA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Informacije o tem, kaj je zahtevano za druge vrste, najdete v tem članku: Kaj so vrste [občutljivih informacij?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  