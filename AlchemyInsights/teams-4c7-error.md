---
title: Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049324"
---
# <a name="4c7-error-in-microsoft-teams"></a>Napaka 4c7 v Microsoft Teams

Do te napake pride, ker Microsoft Teams preverjanje pristnosti obrazcev. Ko uvedete storitve AD FS (Active Directory Federation Services), preverjanje pristnosti obrazcev ni privzeto omogočeno za intranet. Če Windows preverjanje pristnosti ne uspe, ste pozvani k vpisu s preverjanjem pristnosti obrazcev.

Če želite odpraviti to težavo, omogočite preverjanje pristnosti obrazcev s snap-inom AD FS Microsoft Management Console (MMC) v računalniku, ki ima lokalno kopijo imenika Active Directory. To naredite tako: 

1. V podoknu za krmarjenje poiščite Pravilniki **za preverjanje pristnosti.**
2. V **razdelku Dejanja** v podoknu s podrobnostmi izberite Urejanje **globalnega primarnega preverjanja pristnosti.**
3. Na zavihku **Intranet** izberite Preverjanje **pristnosti obrazcev.**
4. Izberite **V redu** (ali **Uporabi).**