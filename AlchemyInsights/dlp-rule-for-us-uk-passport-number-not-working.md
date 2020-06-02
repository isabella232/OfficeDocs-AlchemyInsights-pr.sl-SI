---
title: Pravilo DLP za številko potnega lista ZDA/UK ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507314"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Težave s številkami potnih listov DLP-US/UK

**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP vprašanja z ZDA/UK številke potnega lista**

Ali imate težave s **preprečevanjem izgube podatkov (DLP)** , ki ne deluje za vsebino, ki vsebuje **številko potnega lista ZDA/UK** pri uporabi vrste občutljivih informacij DLP v O365? Če je tako, preverite, ali vsebina vsebuje potrebne informacije za to, kar išče pravilnik DLP, ko je ovrednoten.
  
Na primer, za pravilnik o **številki potnega lista ZDA/UK** , konfigurirani z ravnjo zaupanja 75%, se ocenijo in morajo biti odkrite za pravilo, ki sproži
  
- **[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet števk

- **[Vzorec:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet zaporednih števk

- **[Kontrolna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ni checksum

- **[Definicijo:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Pravilnik DLP je 75% prepričan, da je zaznal to vrsto občutljivih informacij, če v bližini 300 znakov:

  - Funkcija Func_usa_uk_passport poišče vsebino, ki se ujema z vzorcem.

  - Najdena je ključna beseda iz Keyword_passport.

    Na primer, naslednji vzorec bi sprožila za **ZDA/UK številka potnega lista** politike: us passport številka 123456789

Za več informacij o tem, kaj je potrebno za ZDA/UK številka potnega lista, ki se zazna za vašo vsebino, glejte naslednji razdelek v tem članku: [Kaj občutljive vrste informacij IŠČEJO ZDA/UK Passport številka](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Z drugačno vgrajeno vrsto občutljivih informacij si oglejte ta članek za informacije o tem, kaj je potrebno za druge vrste: [Kaj iščejo občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  