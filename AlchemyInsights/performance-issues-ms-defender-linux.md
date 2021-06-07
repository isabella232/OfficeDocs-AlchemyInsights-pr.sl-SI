---
title: Težave z učinkovitostjo delovanja za Microsoft Defender za končno točko v sistemu Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794226"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Težave z učinkovitostjo delovanja za Microsoft Defender za končno točko v sistemu Linux

V tem članku so navodila za določanje težav z učinkovitostjo delovanja za Microsoft Defender for Endpoint v sistemu Linux.

Pomembno je, da najprej preverite, ali je težava, do katere prihaja, odpravljena z [najnovejšo različico.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Če želite začeti raziskovanje, glejte Odpravljanje [težav z učinkovitostjo delovanja za Microsoft Defender for Endpoint v sistemu Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Izključitve

Z izključitevm lahko zmanjšate težave z učinkovitostjo delovanja. Preden začnete, preglejte izključitve, da bo vsa dodatna tveganja znana in dokumentirana.

Če želite več informacij, glejte [Konfiguracija in preverjanje veljavnosti izključitev za Microsoft Defender for Endpoint on Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Če morate izključiti & datotek ali map, ki so vse v isti kopeti, je morda lažje, če izključite točko konjene. S februarsko izdajo 101.22.80 lahko izključite celotno točko konjene.

Če je na primer /mnt/varnostna kopija gora, lahko na izključen seznam dodate /mnt/backup tako, da zaženete ta ukaz:

`$ mdatp exclusion folder add –path /mnt/backup`

**Opomba:** z dodajanjem izključitev povečate tveganje, da zlonamerna programska oprema ne bo zaznana, zato jo morate obravnavati in uvesti previdno.

## <a name="need-help"></a>Potrebujete pomoč?

Če želite pomoč na najučinkovitejši način, zberite diagnostične podatke, preden odprete primer podpore.
