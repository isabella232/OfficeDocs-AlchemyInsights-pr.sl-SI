---
title: Težave z odstranjevanjem nenajavne ali izločitev naprave iz inventarja naprave
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892019"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Težave z odstranjevanjem nenajavne ali izločitev naprave iz inventarja naprave

Microsoft Defender za končno točko trenutno ne omogoča ročnega odstranjevanja zapisa naprave za nenajavno ali izločitev naprave iz inventarja naprav.

Zaradi varnostnih razlogov naprava ostane na portalu kot zgodovinski zapis do 180 dni. Podatki o napravi pa so purged v skladu s konfigurirano obdobjem hranjenja.

**Opomba:** Nenatisljena ali izločitev naprave po sedmih dneh **samodejno** preklopi na stanje »Nedejaven«. Poleg tega naprave, ki v zadnjih 30 dneh niso aktivne, niso upoštevane v podatkih, ki odražajo vrednost vaše organizacije upravljanje groženj in ranljivosti izpostavljenosti ali Microsoftovo oceno varnosti za naprave.
 
Če še vedno ne želite videti določenih naprav v pogledu zaloge naprave, poskusite s posneti oznako naprave, da filtrirate izločitev naprave iz pogleda inventarja naprav.

Če želite več informacij, si oglejte:

[Offboard devices from the Microsoft Defender for Endpoint service](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Ocena izpostavljenosti v upravljanje groženj in ranljivosti](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Popravljanje neprimernih senzorjev v aplikaciji Microsoft Defender for Endpoint](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Kako učinkovito uporabljati označevanje (1. del)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Kako učinkovito uporabljati označevanje (2. del)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Kako učinkovito uporabljati označevanje (3. del)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




