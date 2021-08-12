---
title: Iskanje in brisanje e-poštnih sporočil v organizaciji
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948899"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Iskanje in brisanje e-poštnih sporočil v organizaciji

Upoštevajte te korake:

1. Če niste globalni skrbnik, morate sporočila, ki jih želite poiskati, dodati v skupino vlog upravitelja **e-odkrivanja** ali vlogo upravljanja iskanja **skladnosti.** Če želite izbrisati sporočila, se morate pridružiti skupini vlog za upravljanje **organizacije** ali vlogi za upravljanje iskanja in **čiščenja.** Dovoljenja za te vloge so dodeljena v središču za varnost in [& za skladnost s predpisi.](https://protection.office.com)
2. [Ustvarite iskanje vsebine in](https://docs.microsoft.com/office365/securitycompliance/content-search) poiščite sporočilo, ki ga želite izbrisati.
3. [Povezovalnik središču za & za skladnost s predpisi PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell) Če uporabljate MFA, si oglejte ta navodila: Povezovalnik središče za varnost in skladnost s predpisi & PowerShell z večkratno [preverjanjem pristnosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Izbrišite sporočilo: zaženite `New-ComplianceSearchAction` ukaz »cmdlet« in izbrišite sporočilo. Izbrisana sporočila so premaknjena v uporabnikovo mapo »Obnovljivi elementi«. Za vzorčni ukaz glejte [3. korak: Brisanje sporočila.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
