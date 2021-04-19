---
title: 'Optični bralnik AIP: namestitev in konfiguracija'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821679"
---
# <a name="aip-scanner-installation-and-configuration"></a>Optični bralnik AIP: namestitev in konfiguracija

**Če želite namestiti optični bralnik AIP, upoštevajte priporočena navodila:**

1. Če nadgrajvate in ne izvajate čistih namestitev, upoštevajte navodila za nadgradnjo optičnega bralnika [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) in za odjemalec za poenoteno označevanje, ki si oglejte nadgradnja optičnega bralnika Azure Information [Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Preverite, ali izpolnjujete vse zahteve [za požarne zidove in nastavitve omrežne infrastrukture.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Prepričajte se, [da so pravilniki nastavljeni](https://docs.microsoft.com/azure/information-protection/configure-policy) na samodejno označevanje ali imajo privzeto oznako v pravilniku.
4. Prepričajte se, da je relevantna vrsta datoteke konfigurirana za oznako/zaščito, kot je opisano v vrstah datotek, ki jih [podpira odjemalec Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Če želite spremeniti privzeto vedenje, upoštevajte ta navodila: [Spreminjanje privzete ravni zaščite datotek.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Preverite, ali ima uporabniški račun, konfiguriran za zagon storitve optičnega bralnika, dovoljenja za dostop do vseh konfiguriranih skladišč.
6. Če imate še vedno težave, izvozite dnevnike optičnega bralnika in jih dodajte na vstopnico za podporo.

**Izvoz dnevnikov programa Azure Information Protection Scanner**

1. Pomaknite se do %localappdata%\Microsoft\MSIP v kontekstu uporabnika, v katerem se izvaja storitev optičnega bralnika.
2. Stisnete vso vsebino v mapo MSIP.
3. Shranite dnevnike na svojo lokacijo in jih priložite zahtevi za storitev.
4. Uporabite lahko tudi [Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Če želite dodatne informacije, glejte:**
- [Uvajanje optičnega bralnika Azure Information Protection za samodejno razvrščanje in zaščito datotek](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Določanje in uporaba parametra žetona za Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Zagon kroga odkrivanja in ogled poročil za optični bralnik](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Pregled dokumentacije za storitev Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Zahteve za storitev Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Prenos odjemalca storitve Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
