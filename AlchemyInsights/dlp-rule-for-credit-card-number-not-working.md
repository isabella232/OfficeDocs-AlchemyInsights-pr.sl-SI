---
title: DLP pravilo za številko kreditne kartice ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704217"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Težave z DLP s številkami kreditnih kartic

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

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
  