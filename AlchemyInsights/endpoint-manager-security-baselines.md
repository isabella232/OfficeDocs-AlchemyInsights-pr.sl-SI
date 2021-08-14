---
title: Endpoint Manager – osnove varnosti
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
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978177"
---
# <a name="endpoint-manager---security-baselines"></a>Endpoint Manager – osnove varnosti

Osnove varnosti so vnaprej konfigurirane skupine nastavitev sistema Windows, ki vam pomagajo uporabiti varnostne nastavitve, ki jih priporočajo ustrezne varnostne skupine. Ta izhodišča je mogoče prilagoditi tako, da zagotavljajo samo želene nastavitve in vrednosti. Za več informacij o varnostnih izhodiščih glejte [Uporaba varnostnih izhodišč za konfiguriranje naprav Windows 10 v Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Trenutno obstajajo osnove za te izdelke:

- Varnostne nastavitve Windows MDM
- Microsoft Defender za končno točko
- Microsoft Edge

Posamezna izhodišča se redno posodabljajo in izdajajo v postopnih različicah. Vsaka različica doda in odstrani nastavitve iz prejšnje različice, da zagotovi, da osnova ustreza trenutnim navodilom. Konzola osnov varnosti v programu Endpoint Security omogoča primerjavo različnih različic, tako da so spremembe vidne od različice do različice.

Za napotke o tem, kako najučinkoviteje spremeniti uporabljeno različico osnove, glejte [Upravljanje varnostnih profilov osnovne linije v Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Po uvedbi osnove varnosti lahko spremljate stanje uvajanja in pregledate nastavitve za vsako napravo posebej.

**Opomba:** Podatki poročanja o napakah za osnove varnosti lahko trajajo do 24 ur, preden se prikažejo od začetne uvedbe do naprave, in do 6 ur za nadaljnje posodobitve. 

Najpogostejši vzrok, da se osnovna nastavitev ne uporablja, je zato, ker se ista nastavitev uporablja v drugačnem profilu. Ta scenarij je mogoče raziskati za določeno napravo tako, da jo izberete v vozlišču Stanje naprave profila osnove varnosti. Če želite izvedeti več, si oglejte [Razreševanje sporov za osnove varnosti](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).