---
title: Omogočanje uporabniku, da sinhronizira osebni račun s službeni račun v Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813407"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Omogočanje uporabniku, da sinhronizira osebni račun s službeni račun v Microsoft Edge

Preverite, ali izpolnjujete te pogoje:

- Podatkovno središče Enterprise State Roaming je omogočeno v skrbniškem središču za Azure Active Directory, ki zahteva naročnino na Azure Active Directory Premium ali Enterprise Mobility + Security (EMS). Če želite več informacij, glejte [Omogočanje gostovanja v državi podjetja Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Izpolnjena sta enega ali oba od teh pogojev:
    - Storitev Azure Information Protection je omogočena za vašega najemnika. Če želite več podrobnosti, [glejte Aktiviranje zaščite storitve Azure Rights Management iz Skrbniško središče za Microsoft 365](/azure/information-protection/activate-office365).
    - Funkcija Azure Active Directory enterprise State Roaming (ESR) je omogočena za katerega koli uporabnika ali najemnika. Če želite več informacij, glejte [Kaj je gostovanje v stanju poslovnega gostovanja?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Če sta AIP in ESR onemogočena, se prikaže sporočilo o napaki, da uporabniki, ki sinhronizirajo, niso na voljo za svoje račune.
