---
title: DLP pravilo za nas številka bančnega računa ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389485"
---
Ali imate težave s **Podatki Loss preprečevanje (DLP)** ne delajo za vsebino, ki vsebuje **Številko bančnega računa ZDA** pri uporabi vrsto DLP občutljive informacije v O365? Če je tako, poskrbite, da vaša vsebina vsebuje potrebne informacije za kaj je politika DLP iščejo, ko je ovrednotena.
  
Na primer, za politike **ZDA številka bančnega računa** , konfiguriran s 85 % stopnjo zaupanja, naslednje ovrednotimo in je treba odkrivati za pravilo, da sproži:
  
- **[Oblika:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 številk

- **[Vzorec:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 zaporednih številk.

- **[Ček:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Ne, ni ne ček

- **[Opredelitev:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika je 75 % prepričana, da je zaznal te vrste občutljivih podatkov, če v bližini 300 znakov:

  - Regularni izraz Regex_usa_bank_account_number najde vsebine, ki se ujema z vzorcem

  - Ključno besedo iz Keyword_usa_Bank_Account je našel.

    Na primer, ta vzorec bi sprožila politike **ZDA številka bančnega računa** : tekoči račun 78344011

Več informacij o tem, kaj je potrebno za **ZDA številka bančnega računa** za vašo vsebino, je mogoče odkriti, glejte naslednji razdelek v tem članku: [Kaj je občutljive vrste informacij poiščite ZDA številka bančnega računa](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Z uporabo vrste različnih vgrajeno občutljive informacije, glejte ta članek za informacije na kaj je potrebno za druge vrste: [Kaj je občutljive vrste informacij iščejo](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  