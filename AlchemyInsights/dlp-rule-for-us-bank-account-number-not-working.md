---
title: Pravilo DLP za številko AMERIŠKEGA bančnega računa ne deluje
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679312"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Težave z DLP s številkami AMERIŠKEGA bančnega računa

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave z DLP s številkami AMERIŠKEGA bančnega računa**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** ne delate za vsebino, ki vsebuje **številko ameriškega bančnega računa** , ko uporabljate vrsto občutljivih podatkov DLP v O365? Če je tako, se prepričajte, da vaša vsebina vsebuje potrebne informacije o tem, kaj išče pravilnik DLP, ko ga ocenite.
  
Na primer, za pravilnik **številka ameriškega bančnega računa** , konfiguriran z ravnjo zaupanja 85%, se ocenijo in jih je treba zaznati, da sproži pravilo:
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 števk

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 zaporednih števk.

- **[Preskusna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ni checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če je v bližini 300 znakov:

  - Regularni izraz Regex_usa_bank_account_number najde vsebino, ki se ujema z vzorcem

  - Najde se ključna beseda iz Keyword_usa_Bank_Account.

    Na primer, naslednji vzorec bi sprožilo za pravilnik o **številu bančnih računov v ZDA** : preverjanje računa 78344011

Če želite več informacij o tem, kaj je potrebno za **številko bančnega računa v ZDA** , ki jo želite zaznati za vašo vsebino, si oglejte ta razdelek v tem članku: [Kaj so občutljive vrste informacij za ameriško številko bančnega računa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Če uporabljate drugačno vgrajeno občutljivo vrsto informacij, si oglejte ta članek za informacije o tem, kaj je zahtevano za druge vrste: [Kaj so videti občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  