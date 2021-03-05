---
title: Težave s ZVOČNO povezavo za zdravje
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483120"
---
# <a name="problem-with-aad-connect-health"></a>Težave s ZVOČNO povezavo za zdravje

- Zagotovite, da imate dovoljenje za izvedbo operacije. Globalni skrbniki imajo privzeto dostop do njih. Poleg tega lahko uporabite [nadzor dostopa](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , ki temelji na vlogi, če želite dodeliti dovoljenje za registracijo plačniku.
- Zagotovite, da so zahtevane končne točke omogočene in niso blokirane zaradi požarnega zidu. Če želite več informacij, glejte [zahteve](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registracija ni mogoča zaradi odhodne komunikacije, ki jo je treba pregledati prek omrežja SSL.
- Preverite, ali ste preverili nastavitve obveščanja za povezavo z zdravjem za Azure AD Connect. Oglejte si nastavitev. S tem [vodnikom](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) lahko razumete, kako konfigurirate nastavitve obvestila za obvestila o zdravju v storitvi Azure ad Connect.
- Če želite izvedeti več o poročilu o sinhronizaciji ZVOČNIh povezav in kako jo prenesti, glejte [poročilo o sinhronizaciji ravni predmeta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Če želite odpraviti težave z zdravstvenimi opozorili, si oglejte [navodila za odpravljanje težav s povezovanjem zdravstvenih podatkov](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) in za pogosta vprašanja o [pogostosti težav s povezovanjem zdravja](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
