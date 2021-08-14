---
title: Težava z AAD Povezovalnik Health
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
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923768"
---
# <a name="problem-with-aad-connect-health"></a>Težava z AAD Povezovalnik Health

- Prepričajte se, da imate dovoljenje za izvajanje operacije. Globalni skrbniki imajo privzeto dostop. Poleg tega lahko s kontrolnikom dostopa [na osnovi vloge](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) dodelite dovoljenje za registracijo sodelavca.
- Prepričajte se, da so zahtevane končne točke omogočene in ne blokirane zaradi požarnega zidu. Za podrobnosti glejte [zahteve.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registracija lahko ne uspe, ker omrežna plast pregleda SSL za odhodno komunikacijo.
- Preverite, ali ste preverili nastavitve obvestil za Azure AD Povezovalnik Health. Preglejte svojo nastavitev. V [tem](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vodniku boste lahko razumeli, kako konfigurirate nastavitve obvestil za obvestila za Azure AD in Povezovalnik stanja storitve.
- Če želite izvedeti več o poročilu o sinhronizaciji Povezovalnik stanje storitve in kako ga prenesete, glejte Poročilo o sinhronizaciji [na ravni predmeta.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Če želite odpraviti težave z opozorili storitve AAD Povezovalnik Health, upoštevajte vodnik za odpravljanje težav za storitev [AAD Povezovalnik](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Opozorila o svežini podatkov o zdravju in za pogosta vprašanja, glejte Pogosta vprašanja o storitvi [AAD Povezovalnik Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
