---
title: Pravilo o dlpciji za številko kreditne kartice ne deluje
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005106"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Težave slpci s kreditno kartico

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**Težave slpci s kreditno kartico**

Ali imate težave s funkcijo za preprečevanje izgube podatkov  **(DLP),** ki ne deluje za vsebino, ki vsebuje številko kreditne kartice, ko uporabljate vrsto občutljivih podatkov za preprečitev izgube podatkov v storitvi O365? V tem primeru se prepričajte, da vsebina vsebuje potrebne informacije za sprožitev pravilnika o DLP, ko se ovrednoti. Na primer, za pravilnik **kreditne** kartice, konfiguriran z ravni zaupanja 85 %, so te ovrednotene in jih je treba zaznati, da pravilo sproži:
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 števk, ki jih je mogoče oblikovati ali neoblikovano (dddddddd) in morajo prevesti preskus Luhn.

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Zelo zapleten in zmogljiv vzorec, ki zazna kartice vseh večjih blagovnih znamk po vsem svetu, vključno z blagovnimi znamkami Visa, MasterCard, Discover Card, JCB, American Express, darilnimi karticami in karticami Ner.

- **[Kontrolna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, kontrolna vsota Luhn

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Pravilnik o DLP je 85 % prepričan, da je zaznal to vrsto občutljivih informacij, če znotraj bližine 300 znakov:

  - Funkcija Func_credit_card najde vsebino, ki se ujema z vzorcem.

  - Velja nekaj od tega:

  - Najde se ključna beseda Keyword_cc_verification iz te vrste.

  - Najde se ključna beseda Keyword_cc_name iz

  - Funkcija Func_expiration_date najde datum v pravi obliki zapisa datuma.

  - Kontrolna vsota prestane

    Za pravilnik o številki kreditne kartice dlp bi na primer sprožili ta vzorec:

  - Visa: 4485 3647 3952 7352
  
  - Poteče: 2/2009

Če želite več informacij o  tem, kaj je zahtevano, da je za vašo vsebino zaznana številka kreditne kartice, si oglejte ta razdelek v tem članku: Kaj vrste občutljivih podatkov look [for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Informacije o tem, kaj je zahtevano za druge vrste, najdete v tem članku: Kaj so vrste [občutljivih informacij?](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  