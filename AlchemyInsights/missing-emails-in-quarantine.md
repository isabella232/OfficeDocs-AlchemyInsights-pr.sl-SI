---
title: Manjkajoča e-poštna sporočila v karanteni
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329678"
---
# <a name="missing-emails-in-quarantine"></a>Manjkajoča e-poštna sporočila v karanteni

Skrbniki si lahko [ogledajo ta sporočila, jih pustijo ali jih izbrišejo](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

V portalu Microsoft 365 Defender pojdite v <https://security.microsoft.com> pregled  \> **karantene.** Če pa se želite neposredno poiskovati **na stran** Karantena, uporabite <https://security.microsoft.com/quarantine> .  

Če želite več informacij o vrednostih iskanja/filtra, ki jih lahko uporabite, glejte Upravljanje sporočil in datotek v karanteni kot [skrbnik v EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Ukazi »cmdlet« za ogled in upravljanje sporočil in datotek v karanteni so:

- [Brisanje-karantenamessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz v karanteno](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Predogled–karantena:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)ta ukaz »cmdlet« je le za sporočila in ne za datoteke iz Sef prilog za SharePoint, OneDrive ali Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
