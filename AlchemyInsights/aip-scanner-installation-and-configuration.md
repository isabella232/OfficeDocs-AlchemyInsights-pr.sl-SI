---
title: 'AIP skener: namestitev in konfiguracija'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358566"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP skener: namestitev in konfiguracija

**Za namestitev optičnega bralnika AIP sledite priporočenim smernicam**:

1. Če nadgrajujete in ne izvajate čiste namestitve, preverite, ali ste sledili smernicam za [nadgradnjo aplikacije Azure Information zaščita](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) in za poenoteni odjemalec za označevanje, glejte [Nadgradnja skenerja za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Preverite, ali ste skladni z vsemi [zahtevami za nastavitve požarne zidove in omrežne infrastrukture](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Prepričajte se, da [so pravilniki nastavljeni](https://docs.microsoft.com/azure/information-protection/configure-policy) na samodejno označevanje ali imajo privzeto oznako v pravilniku.
4. Prepričajte se, da je ustrezna vrsta datoteke konfigurirana za oznako/zaščito, kot je opisano v [vrstah datotek, ki jih podpira odjemalec Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Poleg tega, če želite spremeniti privzeto obnašanje, upoštevajte te smernice: [Spreminjanje privzete ravni zaščite datotek](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Preverite, ali ima uporabniški račun, konfiguriran za zagon storitve optičnega bralnika, dovoljenja za dostop do vseh konfiguriranih skladišč.
6. Če še vedno naletite na težave, prosimo, izvozite dnevnike optičnega bralnika in jih dodajte v vašo podporo vozovnice.

**Izvoz dnevnikov zaščite podatkov Azure**

1. Pluti v%localappdata%\Microsoft\MSIP pod uporabnik zveza tekmovanje v teku radarska antena usluga.
2. Zip vse vsebine pod MSIP mapo.
3. Shranite dnevnike na svojo izbiro lokacije in jih priložite zahtevi za storitev.
4. Uporabite lahko tudi [izvozno-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Za dodatne informacije glejte**:
- [Uvajanje skenerja za zaščito podatkov Azure za samodejno razvrščanje in zaščito datotek](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Določanje in uporaba parametra žetona za» Set-AIPAuthentication «](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Zaženite cikel odkrivanja in si oglejte poročila za optični bralnik](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Preglejte dokumentacijo o varstvu podatkov Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Zahteve za zaščito podatkov Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Prenesite odjemalca za zaščito podatkov Azure](https://www.microsoft.com/download/details.aspx?id=53018)
