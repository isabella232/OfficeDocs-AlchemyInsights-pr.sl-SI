---
title: Pravila za zmanjšanje površine napadov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676443"
---
# <a name="attack-surface-reduction-rules"></a>Pravila za zmanjšanje površine napadov

Izključitev datotek ali map lahko resno zmanjša zaščito, ki jo zagotavljajo pravila za zmanjšanje površine napadov. Datoteke, ki bi jih blokiralo pravilo, se lahko zaženejo, poročilo ali dogodek pa se ne posname. Izključitev velja za vsa pravila, ki dovoljujejo izjeme.

Izključitve ASR uporabljajo enako sintakso kot Microsoft Defender Antivirus izključitve. Če želite več informacij, [glejte Konfiguracija in preverjanje veljavnosti izključitev Microsoft Defender Antivirus pregledih.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Če se želite izogniti težavam, preglejte pogoste napake, ki se [jim morate izogniti pri določanju izključitev.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Izključitve niso podrte z vsemi pravili ASR. Če želite preveriti, ali pravilo podpira izključitve, glejte tabelo Pravila za [zmanjšanje števila napadov.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Pravila za zmanjšanje površine napadov

Površina napadov organizacije vključuje vsa mesta, kjer lahko napadalec ogrozi naprave ali omrežja organizacije. Zmanjšanje števila napadov pomeni zaščito naprav in omrežja organizacije, pri katerem napadalci ostanejo na manj načinov za izvajanje napadov. V pomoč so lahko pravila za zmanjšanje površine napadov v programu Microsoft Defender za končno točko.

Če želite več informacij, si oglejte:

- [Guid pravila »Preslikaj kot pravilo ASR za ime](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Zahteve pravil ASR:
    - [Windows 10 Pro, različica 1709 ali novejša](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, različica 1709 ali novejša](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Strežnik, različica 1803 (polletni kanal) ali novejša različica](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Določite pravilno izključitev, ki jo želite uporabiti

1. Poiščite ID dogodka 1121 ali 1122 v Microsoftovem Windows-Windows Defender/dnevniku delovanja.

1. Ocenite scenarij blokiranja in kontekst ter potrdite, da je treba ta scenarij odblokiran.

1. Preberite vrednost Path (Pot) v podrobnostih dogodka, ki je vrednost, ki določa izključitev.
    - Izključitev naj bo čim bolj stroga.
    - Po potrebi uporabite nadomestni znak (nadomestite na primer »Uporabnik spremenljivka«).

1. Uporabite izključitev glede na potrebe uvajanja. Če želite več informacij, [glejte Prilagajanje pravil za zmanjšanje površine napadov.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Izključitev ni v skladu s

1. Določite, ali pravilo podpira izključitve. Če želite več informacij, glejte [Pravila za zmanjšanje števila napadov.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Preglejte uporabljene izjeme in preverite, ali so v podatkih o dogodku morda tipkarske napake ali nadomestni znaki, ki se narobe tolmačijo. Če želite več informacij, glejte [Podprte vrste izključitev](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. če je vpliv pravila prenizka, premislite o premiku pravila (nazaj) v način nadzora, da izvedete dodatno preverjanje veljavnosti. Če želite več informacij, [glejte Preskus delovanja programa Microsoft Defender for Endpoint v načinu nadzora.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. S tem ukazom zberite podatke podpore, da odprete primer podpore:
    
   ** MDEClientAnalyzer.cmd -v**

    Če želite več informacij, glejte [Težave s računalniki za upravljanje s programom Microsoft Defender za končne točke.](issues-with-onboarding-machines.md)
