---
title: EndPoint Manager – varnostni osnovni načrt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421091"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager – varnostni osnovni načrt

Varnostni osnovni načrt so vnaprej konfigurirane skupine nastavitev sistema Windows, s pomočjo teh nastavitev lahko uporabite varnostne nastavitve, ki jih priporočajo ustrezne varnostne skupine. Te osnovne vrstice je mogoče prilagoditi tako, da zagotavljajo le želene nastavitve in vrednosti. Če želite več informacij o varnostnih osnovnih črtah, glejte Uporaba varnostnih osnovnih načrta [za konfiguracijo naprav s sistemom Windows 10 v storitvi Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Trenutno obstajajo osnovni načrti za te izdelke:

- Varnostne nastavitve sistema Windows MDM
- Microsoft Defender for EndPoint Security
- Microsoft Edge

Vsak osnovni načrt se redno posodablja in izda v postopnih različicah. Vsaka različica doda in odstrani nastavitve iz prejšnje različice in tako zagotovi, da osnovni načrt izpolnjuje trenutne smernice. Konzola »Varnostni osnovni osnovni načrt« v varnosti končne točke omogoča, da se različne različice primerjajo tako, da so spremembe vidne iz različice v različico.

Navodila za najučinkovitejšo spremembo, katera različica osnovnega načrta je uvedena, so v članku Upravljanje profilov osnovnega načrta za varnost [v storitvi Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Ko uvedete varnostni osnovni načrt, lahko spremljate stanje uvajanja in pregledujete nastavitve na osnovi naprav.

**Opomba:** Podatki poročanja za osnovne vrstice lahko trajajo do 24 ur, da se prikažejo od začetne uvedbe do naprave in do 6 ur za dodatne posodobitve. 

Najpogostejši vzrok za neuuporabljena nastavitev osnovnega načrta je, ker se ista nastavitev uporablja v drugem profilu. Ta scenarij lahko raziščete za določeno napravo tako, da to napravo izberete v vozlišču Stanje naprave v profilu varnostnega osnovnega načrta. Če želite več informacij, [glejte Razreševanje sporov za varnostne osnovne načrte.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)