---
title: Pravilo DLP za številko bančnega računa ZDA ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: b032a7c80e8b387114aeda95c4f6af7e57225517
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507350"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP težave z ameriški bančnega računa številke

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP težave z ameriški bančnega računa številke**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko bančnega računa ZDA** pri uporabi vrste občutljivih informacij DLP v O365? Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP, ko je ovrednoten.
  
Na primer, za pravilnik o **številki ameriškega bančnega računa** , ki je konfiguriran z ravnjo zaupanja 85%, se ocenijo naslednje in morajo biti odkrite za pravilo, ki sproži:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 števk

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 zaporednih števk.

- **[Kontrolna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ni checksum

- **[Definicijo:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:

  - Regularni izraz Regex_usa_bank_account_number najde vsebino, ki se ujema z vzorcem

  - Najdena je ključna beseda iz Keyword_usa_Bank_Account.

    Naslednji vzorec bi na primer sprožil pravilnik o **številki bančnega računa ZDA** : preverjanje računa 78344011

Če želite več informacij o tem, kaj je potrebno za iskanje **številke ameriškega bančnega računa** za vašo vsebino, glejte naslednji razdelek v tem članku: [katere vrste občutljivih informacij so na voljo za ŠTEVILKO bančnega računa ZDA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  