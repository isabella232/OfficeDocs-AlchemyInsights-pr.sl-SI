---
title: Pravilo DLP za številko kreditne kartice ne deluje
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679457"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Težave z DLP s številkami kreditnih kartic

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave z DLP s številkami kreditnih kartic**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** ne delate za vsebino, ki vsebuje **številko kreditne kartice** , ko uporabljate vrsto občutljivih podatkov DLP v O365? Če je tako, se prepričajte, da vaša vsebina vsebuje potrebne informacije, da sproži pravilnik DLP, ko ga ocenite. Na primer, za **pravilnik kreditne kartice** , konfiguriran z ravnjo zaupanja 85%, se ocenijo naslednji in jih je treba zaznati, da bo pravilo sprožilo:
  
- **[Oblika:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 števk, ki jih je mogoče formatirati ali neoblikovane (dddddddddddddddd) in morajo opraviti preskus Luhn.

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Zelo zapleteno in robustno vzorec, ki zazna kartice iz vseh glavnih svetovnih blagovnih znamk, vključno z Visa, MasterCard, Discover Card, JCB, American Express, darilne kartice in Diner CARDS.

- **[Preskusna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, Luhn checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če je v bližini 300 znakov:

  - Funkcija Func_credit_card najde vsebino, ki se ujema z vzorcem.

  - Velja nekaj od tega:

  - Najde se ključna beseda iz Keyword_cc_verification.

  - Najdena je ključna beseda iz Keyword_cc_name

  - Funkcija Func_expiration_date najde datum v pravilni obliki zapisa datuma.

  - Izkaznica checksum

    Na primer, naslednji vzorec bi sprožil za DLP številko kreditne kartice:

  - Visa: 4485 3647 3952 7352
  
  - Poteče: 2/2009

Če želite več informacij o tem, kaj potrebujete za **številko kreditne kartice** , ki jo želite zaznati za vašo vsebino, si oglejte ta razdelek v tem članku: [Kaj so občutljive vrste podatkov, ki iščejo kreditno kartico #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Če uporabljate drugačno vgrajeno občutljivo vrsto informacij, si oglejte ta članek za informacije o tem, kaj je zahtevano za druge vrste: [Kaj so videti občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  