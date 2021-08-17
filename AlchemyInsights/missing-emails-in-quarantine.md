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
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892063"
---
# <a name="missing-emails-in-quarantine"></a>Manjkajoča e-poštna sporočila v karanteni

Skrbniki si lahko [ogledajo ta sporočila, jih pustijo ali jih izbrišejo](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

V Microsoft 365 Defender portalu na spletnem <https://security.microsoft.com> mestu , pojdite v pregled  \> **karantene.** Če pa se želite neposredno po vrniti na stran **Karantena,** uporabite <https://security.microsoft.com/quarantine> .  

Če želite več informacij o vrednostih iskanja/filtra, ki jih lahko uporabite, glejte Upravljanje sporočil in datotek v karanteni kot [skrbnik v EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Ukazi »cmdlet« za ogled in upravljanje sporočil in datotek v karanteni so:

- [Brisanje-karantenamessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz v karanteno](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Predogled-karantena:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)ta ukaz »cmdlet« je le za sporočila in ne za datoteke iz prilog Sef za SharePoint, OneDrive ali Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
